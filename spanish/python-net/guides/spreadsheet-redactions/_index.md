---
title: "Redacciones de hojas de cálculo"
linkTitle: "Spreadsheet redactions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Este artículo muestra cómo la API de redacción de Python permite redactar datos de naturaleza sensible o privada de sus formatos de documento de hoja de cálculo XLS, XLSX, ODS y otros."
type: docs
url: /es/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction permite redactar datos de naturaleza sensible o privada de sus formatos de documento de hoja de cálculo XLS, XLSX, ODS y otros. Consulte la lista completa en el artículo [formatos de documento compatibles]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Especifique las opciones de redacción
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Cargue la hoja de cálculo que será redactada
    with Redactor("./sample.xlsx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(ex_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` es el archivo de ejemplo utilizado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) para descargarlo.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
