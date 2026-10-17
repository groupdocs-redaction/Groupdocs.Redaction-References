---
title: "Annoteringsrödaktioner"
linkTitle: "Annotation redactions"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Denna artikel visar implementeringen av annoteringsrödaktion för dokument i olika format som PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX och andra."
type: docs
url: /sv/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


Med GroupDocs.Redaction API kan du tillämpa annoteringsrödaktioner för dokument i olika format som PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX och andra. Se fullständig lista i artikeln [supported document formats]() .

GroupDocs.Redactions tillhandahåller ett flexibelt API som möjliggör att ta bort känslig data från annoteringstext, eller att helt ta bort annotationer med ett reguljärt uttryck.

## Remove annotations (comments etc)

Du kan använda GroupDocs.Redaction för att ta bort alla eller specifika kommentarer och andra anteckningar från dokumentet. Till exempel kan vi ta bort alla kommentarer från dokumentet, som innehåller texter som "use", "show" eller "describe" i dess kropp:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Ange raderingsalternativen för att ta bort anteckningar som matchar mönstret
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Läs in dokumentet som ska raderas
    with Redactor("./annotated.xlsx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(a_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) för att ladda ner den.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

Du kan använda konstruktorn utan argument för att ta bort alla anteckningar i dokumentet.

## Redact annotations

Istället för att ta bort alla eller specifika anteckningar kan du ta bort känslig data från anteckningstexten. Till exempel kan vi ta bort alla omnämnanden av "John" i det givna dokumentet, t.ex.:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Ange raderingsalternativen: sökmönster och ersättningssträng
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Läs in dokumentet som ska raderas
    with Redactor("./annotated.xlsx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(a_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) för att ladda ner den.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
