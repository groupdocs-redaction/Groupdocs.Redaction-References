---
title: "Annotatie-redacties"
linkTitle: "Annotation redactions"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Dit artikel toont de implementatie van annotatiereductie voor documenten van verschillende formaten zoals PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX en andere."
type: docs
url: /nl/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


Met de GroupDocs.Redaction API kunt u annotatiereducties toepassen op documenten van verschillende formaten zoals PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX en andere. Zie de volledige lijst in het artikel [ondersteunde documentformaten]().

GroupDocs.Redactions biedt een flexibele API die het mogelijk maakt om gevoelige gegevens uit annotatietekst te verwijderen, of annotaties volledig te verwijderen met een reguliere expressie.

## Remove annotations (comments etc)

U kunt GroupDocs.Redaction gebruiken om alle of specifieke opmerkingen en andere annotaties uit het document te verwijderen. Bijvoorbeeld, we kunnen alle opmerkingen uit het document verwijderen die teksten bevatten zoals "use", "show" of "describe" in de inhoud:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Specificeer de redactie-opties om annotaties te verwijderen die overeenkomen met het patroon
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Laad het te redigeren document
    with Redactor("./annotated.xlsx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(a_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) om het te downloaden.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

U kunt de constructor zonder argumenten gebruiken om alle annotaties binnen het document te verwijderen.

## Redact annotations

In plaats van alle of specifieke annotaties te verwijderen, kun je gevoelige gegevens uit de annotatietekst verwijderen. Bijvoorbeeld, we kunnen alle vermeldingen van \"John\" in het gegeven document verwijderen, bijv.:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Specificeer de redactie‑opties: zoekpatroon en vervangingsstring
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Laad het te redigeren document
    with Redactor("./annotated.xlsx") as redactor:
        # Pas de redactie toe
        result = redactor.apply(a_red)

        # Sla het geredigeerde document op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) om het te downloaden.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
