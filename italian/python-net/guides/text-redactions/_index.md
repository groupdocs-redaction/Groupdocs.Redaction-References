---
title: "Redazione del testo"
linkTitle: "Text redaction"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Questo articolo spiega come l'API di redazione Python consenta di redigere facilmente dati di natura sensibile o privata dai tuoi documenti. Puoi applicare la redazione del testo usando una frase esatta o un'espressione regolare per documenti di diversi formati come PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX e altri."
type: docs
url: /it/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction consente di redigere facilmente dati di natura sensibile o privata dai tuoi documenti. Il caso di redazione più comune è rimuovere un testo da un documento.

Con l'API GroupDocs.Redaction è possibile applicare la redazione del testo usando una frase esatta o [espressione regolare](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) per documenti di diversi formati come PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX e altri. Vedi l'elenco completo nell'articolo [formati di documento supportati]().

## Use exact phrase redaction

Nell'esempio seguente, applichiamo la redazione testuale, sostituendo la frase esatta personale "John Doe" con "\[personal\]" (o qualsiasi codice di esenzione):

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Specifica le opzioni di redazione
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione
        result = redactor.apply(ex_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` è il file di esempio utilizzato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) per scaricarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

Per impostazione predefinita, la ricerca della frase esatta non distingue tra maiuscole e minuscole. Per una redazione sensibile al maiuscolo/minuscolo, esiste un parametro del costruttore e la relativa proprietà pubblica:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Abilita il confronto sensibile al maiuscolo/minuscolo
    case_sensitive = True

    # Specifica le opzioni di redazione
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione
        result = redactor.apply(ex_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` è il file di esempio utilizzato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) per scaricarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Se hai bisogno di una casella colorata sopra il testo redatto, puoi usare il colore invece della stringa di sostituzione. La redazione cancellerà il testo corrispondente e inserirà un rettangolo del colore specificato al posto del testo redatto:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Definisci il colore della casella di redazione
    color = Color.from_argb(255, 220, 20, 60)

    # Specifica le opzioni di redazione
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione
        result = redactor.apply(ex_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` è il file di esempio utilizzato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) per scaricarlo.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

Potresti dover applicare la redazione a un documento da destra a sinistra, come l'arabo o l'ebraico. L'esempio seguente dimostra come applicare ExactPhraseRedaction a un documento PDF in arabo:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # Specifica le opzioni di redazione con una frase in arabo
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Carica il documento da redigere
    with Redactor("./arabic.pdf") as redactor:
        # Applica la redazione
        result = redactor.apply(ex_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` è il file di esempio usato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) per scaricarlo.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

Dietro le quinte, la redazione "frase esatta" funziona tramite espressioni regolari, che sono l'approccio di base per la redazione. Nell'esempio seguente, rimuoviamo qualsiasi testo che corrisponde a "2 cifre, spazio o niente, 2 cifre, di nuovo spazio e 6 cifre" con una casella di colore blu:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Definisci il colore della casella di redazione
    color = Color.from_argb(255, 220, 20, 60)

    # Specifica le opzioni di redazione
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione
        result = redactor.apply(reg_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` è il file di esempio utilizzato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) per scaricarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Se hai bisogno di redigere un intero paragrafo, potresti dover utilizzare RegexRedaction. L'esempio seguente dimostra come redigere l'intero paragrafo in un documento PDF:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Definisci il colore della casella di redazione
    color = Color.from_argb(255, 220, 20, 60)

    # Specifica le opzioni di redazione che corrispondono a un intero paragrafo
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Carica il documento da redigere
    with Redactor("./sample.pdf") as redactor:
        # Applica la redazione
        result = redactor.apply(reg_red)

        # Salva il documento redatto accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` è il file di esempio usato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) per scaricarlo.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
