---
title: "Textredaktion"
linkTitle: "Text redaction"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Dieser Artikel erklärt, wie die Python‑Redaktion‑API es Ihnen ermöglicht, Daten sensibler oder privater Art aus Ihren Dokumenten einfach zu redigieren. Sie können Textredaktion mithilfe einer genauen Phrase oder eines regulären Ausdrucks für Dokumente verschiedener Formate wie PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX und andere anwenden."
type: docs
url: /de/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction ermöglicht das einfache Redigieren von Daten sensibler oder privater Art aus Ihren Dokumenten. Der häufigste Anwendungsfall für Redaktionen ist das Entfernen von Text aus einem Dokument.

Mit der GroupDocs.Redaction API können Sie Textredaktion mittels genauer Phrase oder [regular expression](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) für Dokumente verschiedener Formate wie PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX und andere anwenden. Die vollständige Liste finden Sie im Artikel [supported document formats]().

## Use exact phrase redaction

Im folgenden Beispiel wenden wir eine Textredaktion an, indem wir die persönliche genaue Phrase \"John Doe\" durch \"\\[personal\\]\" (oder einen beliebigen Befreiungscode) ersetzen:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Geben Sie die Redaktionsoptionen an
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(ex_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) zum Herunterladen.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

Standardmäßig ist die Suche nach exakter Phrase nicht case-sensitive. Für eine case-sensitive Redaktion gibt es einen Konstruktorparameter und die entsprechende öffentliche Eigenschaft:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Case-sensitive Übereinstimmung aktivieren
    case_sensitive = True

    # Geben Sie die Redaktionsoptionen an
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(ex_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) zum Herunterladen.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Wenn Sie eine farbige Box über dem redigierten Text benötigen, können Sie anstelle des Ersetzungs-Strings die Farbe verwenden. Die Redaktion löscht den gefundenen Text und setzt ein Rechteck der angegebenen Farbe anstelle des redigierten Textes ein:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Definieren Sie die Farbe der Redaktions-Box
    color = Color.from_argb(255, 220, 20, 60)

    # Geben Sie die Redaktionsoptionen an
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(ex_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) zum Herunterladen.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

Möglicherweise müssen Sie eine Redaktion auf ein Rechts-nach-Links-Dokument anwenden, z. B. Arabisch oder Hebräisch. Das folgende Beispiel zeigt, wie man ExactPhraseRedaction auf ein arabisches PDF-Dokument anwendet:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # Geben Sie die Redaktionsoptionen mit einer arabischen Phrase an
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./arabic.pdf") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(ex_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) zum Herunterladen.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

Im Hintergrund funktioniert die \"exact phrase\"-Redaktion über reguläre Ausdrücke, die die grundlegende Methode für Redaktionen darstellen. Im folgenden Beispiel entfernen wir jeden Text, der \"2 Ziffern, optional ein Leerzeichen, 2 Ziffern, erneut ein Leerzeichen und 6 Ziffern\" entspricht, und ersetzen ihn durch eine blaue Farbbox:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Definieren Sie die Farbe der Redaktions-Box
    color = Color.from_argb(255, 220, 20, 60)

    # Geben Sie die Redaktionsoptionen an
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(reg_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) zum Herunterladen.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Wenn Sie einen gesamten Absatz redigieren müssen, sollten Sie möglicherweise auch RegexRedaction verwenden. Das folgende Beispiel zeigt, wie man den gesamten Absatz in einem PDF-Dokument redigiert:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Definieren Sie die Farbe der Redaktions-Box
    color = Color.from_argb(255, 220, 20, 60)

    # Geben Sie die Redaktionsoptionen an, die einen gesamten Absatz matchen
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.pdf") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(reg_red)

        # Speichern Sie das redigierte Dokument neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) zum Herunterladen.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
