---
title: "Hallo, Welt!"
linkTitle: "Hello, World!"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Starten Sie schnell mit GroupDocs.Redaction für Python über .NET, indem Sie ein einfaches Beispiel erstellen und ausführen."
type: docs
url: /de/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
Ein \"Hallo, Welt!\"-Beispiel ist häufig der erste Schritt beim Erkunden von GroupDocs.Redaction für Python über .NET. Es dient als einfacher Test, um zu bestätigen, dass Ihre Entwicklungsumgebung korrekt eingerichtet ist und die Bibliothek wie erwartet funktioniert.

## Overview
GroupDocs.Redaction für Python über .NET ermöglicht das Suchen, Redigieren und Entfernen sensibler Informationen aus verschiedenen Dokumentformaten. Eine breite Palette von [unterstützten Formaten](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) macht es für unterschiedliche Anwendungsfälle vielseitig.

## How to redact a document
Die folgenden Schritte zeigen, wie Sie sensible Informationen aus einem Dokument mit GroupDocs.Redaction für Python über .NET redigieren:

1. Importieren Sie die benötigten `groupdocs.redaction`‑Klassen.
2. Beschreiben Sie die Redaktion (hier ein genauer Ausdruck, der durch ein farbiges Feld ersetzt werden soll).
3. Instanziieren Sie einen [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) mit dem Pfad zum Beispiel-Dokument.
4. Wenden Sie die Redaktion an.
5. Speichern Sie das Ergebnis.

## Complete example
Das nachstehende Beispiel ersetzt jedes Vorkommen des Ausdrucks \"John Doe\" durch ein halbtransparentes rotes Feld und speichert das redigierte Dokument:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # Zeichnen Sie ein halbtransparentes rotes Feld über jedes Vorkommen von \"John Doe\"
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Laden Sie das Dokument, wenden Sie die Redaktion an und speichern Sie das Ergebnis
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` ist die in diesem Beispiel verwendete Beispieldatei. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx), um sie herunterzuladen.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

Dieses Beispiel rastert das Ergebnis in ein PDF mit dem Namen `sample_redacted.pdf`, sodass der redigierte Inhalt nicht wiederhergestellt werden kann (`save()` rastert standardmäßig in PDF; die Option `redacted_file_suffix` steuert lediglich den Ausgabename). Um stattdessen das Originalformat beizubehalten, setzen Sie `rasterize_to_pdf = False`.

## Additional resources
Dieses Beispiel verweist auf die GroupDocs.Redaction für Python via .NET [code samples](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/).
