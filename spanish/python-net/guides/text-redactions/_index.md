---
title: "Redacción de texto"
linkTitle: "Text redaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Este artículo explica cómo la API de redacción de Python le permite redactar fácilmente datos de naturaleza sensible o privada de sus documentos. Puede aplicar redacción de texto usando una frase exacta o una expresión regular para documentos de diferentes formatos como PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX y otros."
type: docs
url: /es/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction permite redactar fácilmente datos de naturaleza sensible o privada de sus documentos. El caso de redacción más popular es eliminar un texto de un documento.

Con la API de GroupDocs.Redaction puedes aplicar redacción de texto usando una frase exacta o [expresión regular](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) para documentos de diferentes formatos como PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX y otros. Consulte la lista completa en el artículo [formatos de documentos compatibles]().

## Use exact phrase redaction

En el ejemplo a continuación, aplicamos redacción textual, reemplazando la frase exacta personal "John Doe" con "\[personal\]" (o cualquier código de exención):

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Especifique las opciones de redacción
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(ex_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` es el archivo de ejemplo usado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) para descargarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

Por defecto, la búsqueda de frase exacta no distingue entre mayúsculas y minúsculas. Para una redacción sensible a mayúsculas, hay un parámetro del constructor y una propiedad pública correspondiente:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Habilitar coincidencia sensible a mayúsculas
    case_sensitive = True

    # Especifique las opciones de redacción
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(ex_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` es el archivo de ejemplo usado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) para descargarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Si necesita un cuadro de color sobre el texto redactado, puede usar color en lugar de la cadena de reemplazo. La redacción borrará el texto coincidente y colocará un rectángulo del color especificado en lugar del texto redactado:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Definir el color del cuadro de redacción
    color = Color.from_argb(255, 220, 20, 60)

    # Especifique las opciones de redacción
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(ex_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` es el archivo de ejemplo usado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) para descargarlo.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

Es posible que necesite aplicar redacción a un documento de derecha a izquierda, como árabe o hebreo. El siguiente ejemplo muestra cómo aplicar ExactPhraseRedaction a un documento PDF en árabe:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # Especifique las opciones de redacción con una frase en árabe
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./arabic.pdf") as redactor:
        # Aplicar la redacción
        result = redactor.apply(ex_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` es el archivo de ejemplo usado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) para descargarlo.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

Detrás de escena, la redacción de \"frase exacta\" funciona mediante expresiones regulares, que son el enfoque básico para la redacción. En el ejemplo a continuación, redactamos cualquier texto que coincida con \"2 dígitos, espacio o nada, 2 dígitos, nuevamente espacio y 6 dígitos\" con un cuadro de color azul:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Definir el color del cuadro de redacción
    color = Color.from_argb(255, 220, 20, 60)

    # Especifique las opciones de redacción
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(reg_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` es el archivo de ejemplo usado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) para descargarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Si necesita redactar un párrafo completo, también podría necesitar usar RegexRedaction. El siguiente ejemplo muestra cómo redactar todo el párrafo en un documento PDF:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Definir el color del cuadro de redacción
    color = Color.from_argb(255, 220, 20, 60)

    # Especifique las opciones de redacción que coincidan con un párrafo completo
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./sample.pdf") as redactor:
        # Aplicar la redacción
        result = redactor.apply(reg_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` es el archivo de ejemplo usado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) para descargarlo.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
