---
title: "Metadataredigeringar"
linkTitle: "Metadata redactions"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Denna artikel visar hur Python redaction API låter dig ersätta eller ta bort metadata med hjälp av filter eller sökning med reguljära uttryck."
type: docs
url: /sv/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


Med GroupDocs.Redaction API kan du tillämpa metadataredigeringar för dokument i olika format som PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX och andra. Se fullständig lista i artikeln [supported document formats]().

GroupDocs.Redactions erbjuder ett flexibelt API som möjliggör att ersätta eller ta bort metadata med filter eller sökning med reguljära uttryck.

## Filter metadata

Basfunktionalitet för alla redigeringar, härledd från basklassen [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/), är *metadata filtering* och den är obligatorisk för metadataredigeringar. Den använder den flaggade uppräkningen [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/), som innehåller objekt för de vanligaste metadata‑posterna. Du kan sätta filtret till *All*, eller någon kombination av metadata. Till exempel sätter exemplet nedan filtret till *Author*, *Manager* och *NameOfApplication* – för textuell redigering eller rensning av dem:

```python
# redigering härledd från MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

Nedan är tabellen med fullständig lista över [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) objekt:

| Filter | Numeriskt värde | Beskrivning |
| --- | --- | --- |
| *None* | 0 | Tom filterinställning, matchar inga metadataobjekt |
| *Author* | 1 | Författare till dokumentet |
| *Kategori* | 2 | Kategori för dokumentet |
| *Kommentarer* | 4 | Dokumentkommentar |
| *Företag* | 8 | Företag för författaren |
| *Innehållsstatus* | 16 | Innehållsstatus |
| *SkapadTid* | 32 | Skapad tid |
| *HyperlänkBas* | 64 | Hyperlänkbas |
| *SenastUtskriven* | 128 | Datum och tid för senaste utskrift |
| *SenastSparadAv* | 256 | Senast sparad av användaren |
| *LastSavedTime* | 1024 | Senast sparade datum och tid |
| *NameOfApplication* | 2048 | Namn på programmet där dokumentet skapades |
| *Manager* | 4096 | Författarens chefsnamn |
| *RevisionNumber* | 8192 | Revisionsnummer |
| *Subject* | 16384 | Dokumentets ämne |
| *Template* | 32768 | Dokumentmallens namn |
| *Title* | 65536 | Dokumenttitel |
| *TotalEditingTime* | 131072 | Total redigeringstid |
| *Version* | 262144 | Dokumentets version |
| *Beskrivning* | 524288 | Dokumentets beskrivning |
| *Nyckelord* | 1048576 | Dokumentets nyckelord |
| *Innehållstyp* | 2097152 | Innehållstyp |
| *Alla* | 2147483647 | Alla typer av metadataobjekt |

## Clean metadata

Du kan ersätta all eller specifik metadata i dokumentet med tomma (tomma eller minimala) värden med hjälp av klassen [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) . Exemplet nedan rensar alla egenskaper i dokumentet:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Ange raderingsalternativen för att radera all metadata
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(met_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) för att ladda ner den.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

Du kan ange [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) eller använda standardkonstruktorn för att rensa all metadata i det angivna dokumentet, Custom - för att rensa alla anpassade metadatafält.

## Redact metadata

Du kan använda [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) för att ta bort känslig data från dokumentets metadata med hjälp av reguljära uttryck. Till exempel kan vi ta bort varje förekomst av "Company Ltd.":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Ange raderingsalternativen: sökmönster och ersättningssträng
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(met_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) för att ladda ner den.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

Det första argumentet är ett reguljärt uttryck, det andra är en ersättningssträng. Du kan också ange räckvidden för raderingen genom att ställa in filter, t.ex. till [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). - det kommer att låta reguljära uttryckens matchningar vara orörda i alla metadataobjekt, förutom egenskapen "Company":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Ange raderingsalternativen: sökmönster och ersättningssträng
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Begränsa raderingsomfånget till endast Company-metadataobjektet
    met_red.filter = MetadataFilters.COMPANY

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(met_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) för att ladda ner den.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Alla metadataredigeringar tillämpas på varje metadataobjekt separat, och även om redigeringen av ett metadataobjekt misslyckas, kommer resten av metadataobjekten att uppdateras. Du kan hitta en lista över misslyckade, överhoppade (avvisade) metadataobjekt och orsakerna till detta i egenskapen [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) i [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
