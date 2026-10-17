---
title: "Textmaskering"
linkTitle: "Text redaction"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Den här artikeln förklarar hur Python redaction API låter dig enkelt maskera data av känslig eller privat natur i dina dokument. Du kan tillämpa textmaskering med exakt fras eller reguljära uttryck för dokument i olika format som PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX och andra."
type: docs
url: /sv/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction gör det enkelt att maskera data av känslig eller privat natur i dina dokument. Det vanligaste maskeringsfallet är att ta bort text från ett dokument.

Med GroupDocs.Redaction API kan du tillämpa textmaskering med exakt fras eller [reguljärt uttryck](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) för dokument i olika format som PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX och andra. Se hela listan i artikeln [supported document formats]().

## Use exact phrase redaction

I exemplet nedan tillämpar vi textmaskering och ersätter den personliga exakta frasen "John Doe" med "\[personal\]" (eller någon undantagskod):

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Ange redigeringsalternativen
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(ex_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) för att ladda ner den.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

Som standard är sökningen efter exakt fras skiftlägesokänslig. För en skiftlägeskänslig redigering finns en konstruktörsparameter och motsvarande publik egenskap:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Aktivera skiftlägeskänslig matchning
    case_sensitive = True

    # Ange redigeringsalternativen
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(ex_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) för att ladda ner den.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Om du behöver en färgad ruta över den redigerade texten kan du använda färg istället för ersättningssträng. Redigeringen kommer att radera matchande text och placera en rektangel i den angivna färgen i stället för den redigerade texten:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Definiera färgen på redigeringsrutan
    color = Color.from_argb(255, 220, 20, 60)

    # Ange redigeringsalternativen
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(ex_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) för att ladda ner den.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

Du kan behöva tillämpa redigering på ett dokument som skrivs från höger till vänster, såsom arabiska eller hebreiska. Följande exempel visar hur man använder ExactPhraseRedaction på ett arabiskt PDF-dokument:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # Ange redigeringsalternativen med en arabisk fras
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./arabic.pdf") as redactor:
        # Applicera maskeringen
        result = redactor.apply(ex_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) för att ladda ner den.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

Bakom kulisserna fungerar "exact phrase"-redigering via reguljära uttryck, vilket är grundmetoden för redigering. I exemplet nedan raderar vi all text som matchar "2 siffror, mellanslag eller inget, 2 siffror, återigen mellanslag och 6 siffror" med en blå färgad ruta:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Definiera färgen på redigeringsrutan
    color = Color.from_argb(255, 220, 20, 60)

    # Ange redigeringsalternativen
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera maskeringen
        result = redactor.apply(reg_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) för att ladda ner den.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Om du behöver redigera ett helt stycke kan du också behöva använda RegexRedaction. Följande exempel visar hur man redigerar hela stycket i ett PDF-dokument:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Definiera färgen på redigeringsrutan
    color = Color.from_argb(255, 220, 20, 60)

    # Ange redigeringsalternativen som matchar ett helt stycke
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.pdf") as redactor:
        # Applicera maskeringen
        result = redactor.apply(reg_red)

        # Spara det redigerade dokumentet bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) för att ladda ner den.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
