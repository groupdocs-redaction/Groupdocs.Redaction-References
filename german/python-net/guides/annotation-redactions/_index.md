---
title: "Anmerkungsredaktionen"
linkTitle: "Annotation redactions"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Dieser Artikel zeigt die Implementierung der Anmerkungsredaktion für Dokumente verschiedener Formate wie PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX und andere."
type: docs
url: /de/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


Mit der GroupDocs.Redaction API können Sie Anmerkungsredaktionen für Dokumente verschiedener Formate wie PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX und andere anwenden. Siehe die vollständige Liste im Artikel [supported document formats]().

GroupDocs.Redactions bietet eine flexible API, die das Entfernen sensibler Daten aus Anmerkungstexten oder das vollständige Entfernen von Anmerkungen mittels regulärem Ausdruck ermöglicht.

## Remove annotations (comments etc)

Sie können GroupDocs.Redaction verwenden, um alle oder bestimmte Kommentare und andere Anmerkungen aus dem Dokument zu entfernen. Zum Beispiel können wir alle Kommentare aus dem Dokument entfernen, die Texte wie \"use\", \"show\" oder \"describe\" im Inhalt enthalten:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Geben Sie die Redaktionsoptionen an, um Anmerkungen zu löschen, die dem Muster entsprechen
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Laden Sie das zu redigierende Dokument
    with Redactor("./annotated.xlsx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(a_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) zum Herunterladen.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

Sie können den Konstruktor ohne Argumente verwenden, um alle Anmerkungen im Dokument zu entfernen.

## Redact annotations

Anstatt alle oder bestimmte Anmerkungen zu entfernen, können Sie sensible Daten aus dem Anmerkungstext entfernen. Zum Beispiel können wir alle Erwähnungen von \"John\" im gegebenen Dokument entfernen, z. B.:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Geben Sie die Redaktionsoptionen an: Suchmuster und Ersetzungszeichenfolge
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Laden Sie das zu redigierende Dokument
    with Redactor("./annotated.xlsx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(a_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) zum Herunterladen.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
