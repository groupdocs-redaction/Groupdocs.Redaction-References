---
title: "Metadata‑redacties"
linkTitle: "Metadata redactions"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Dit artikel laat zien hoe de Python redactie‑API u in staat stelt metadata te vervangen of te verwijderen met behulp van filters of zoeken met reguliere expressies."
type: docs
url: /nl/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


Met de GroupDocs.Redaction API kunt u metadata‑redacties toepassen op documenten van verschillende formaten zoals PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX en andere. Zie de volledige lijst in het artikel [supported document formats]().

GroupDocs.Redactions biedt een flexibele API die het mogelijk maakt metadata te vervangen of te verwijderen met behulp van filters of zoeken met reguliere expressies.

## Filter metadata

Basisfunctionaliteit voor alle redacties, afgeleid van de basisklasse [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) is *metadata filtering* en is verplicht voor metadata‑redacties. Het maakt gebruik van de gemarkeerde enumeratie [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/), die items bevat voor de meest voorkomende metadata‑vermeldingen. U kunt de filter instellen op *All*, of op een combinatie van metadata. Bijvoorbeeld, het onderstaande voorbeeld stelt de filter in op *Author*, *Manager* en *NameOfApplication* – voor tekstuele redacties of om ze te verwijderen:

```python
# redactie afgeleid van MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

Hieronder staat de tabel met de volledige lijst van [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) items:

| Filter | Numerieke waarde | Beschrijving |
| --- | --- | --- |
| *None* | 0 | Lege filterinstelling, komt niet overeen met metadata‑items |
| *Author* | 1 | Auteur van het document |
| *Categorie* | 2 | Categorie van het document |
| *Opmerkingen* | 4 | Documentopmerking |
| *Bedrijf* | 8 | Bedrijf van de auteur |
| *InhoudStatus* | 16 | Inhoudstatus |
| *Creatietijd* | 32 | Creatietijd |
| *Hyperlinkbasis* | 64 | Hyperlinkbasis |
| *LaatsteAfdruk* | 128 | Datum en tijd van laatste afdruk |
| *LaatstOpgeslagenDoor* | 256 | Laatst opgeslagen door gebruiker |
| *LastSavedTime* | 1024 | Datum en tijd van laatste opslag |
| *NameOfApplication* | 2048 | Naam van de applicatie waarin het document is gemaakt |
| *Manager* | 4096 | Naam van de manager van de auteur |
| *RevisionNumber* | 8192 | Revisienummer |
| *Subject* | 16384 | Onderwerp van het document |
| *Template* | 32768 | Naam van het documentsjabloon |
| *Title* | 65536 | Documenttitel |
| *TotalEditingTime* | 131072 | Totale bewerkingstijd |
| *Versie* | 262144 | Versie van het document |
| *Beschrijving* | 524288 | Beschrijving van het document |
| *Trefwoorden* | 1048576 | Trefwoorden van het document |
| *ContentType* | 2097152 | Inhoudstype |
| *Alle* | 2147483647 | Alle soorten metadata-items |

## Clean metadata

U kunt alle of specifieke metadata in het document vervangen door lege (blanco of minimale) waarden met behulp van de klasse [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) . Het voorbeeld hieronder maakt alle eigenschappen van het document leeg:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Specificeer de redactie‑opties om alle metadata te wissen
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(met_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik op [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) om het te downloaden.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

U kunt [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) opgeven of de standaardconstructor gebruiken om alle metadata in het opgegeven document leeg te maken, Custom – om alle aangepaste metadata‑items te wissen.

## Redact metadata

U kunt [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) gebruiken om gevoelige gegevens uit de metadata van het document te verwijderen met behulp van reguliere expressies. Bijvoorbeeld, we kunnen elke vermelding van "Company Ltd." verwijderen:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Specificeer de redactie‑opties: zoekpatroon en vervangingsstring
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(met_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik op [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) om het te downloaden.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

Het eerste argument is een reguliere expressie, het tweede is een vervangingsstring. U kunt ook de scope voor redactie instellen door een filter te definiëren, bijvoorbeeld naar [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). - dit laat de overeenkomsten van de reguliere expressies ongewijzigd in alle metadata‑items, behalve de eigenschap "Company":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Specificeer de redactie‑opties: zoekpatroon en vervangingsstring
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Beperk de redactie‑scope tot alleen het Company‑metadata‑item
    met_red.filter = MetadataFilters.COMPANY

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(met_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik op [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) om het te downloaden.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Alle metadata‑redacties worden afzonderlijk op elk metadata‑item toegepast, en zelfs als de redactie van een metadata‑item mislukt, worden de overige metadata‑items bijgewerkt. U kunt een lijst met mislukte, overgeslagen (afgewezen) metadata‑items en de redenen daarvoor vinden in de eigenschap [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) van [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
