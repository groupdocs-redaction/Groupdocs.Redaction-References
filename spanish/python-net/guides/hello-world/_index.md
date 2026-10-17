---
title: "¡Hola, Mundo!"
linkTitle: "Hello, World!"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Comience rápidamente con GroupDocs.Redaction para Python a través de .NET creando y ejecutando un ejemplo sencillo."
type: docs
url: /es/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
Un ejemplo "¡Hola, Mundo!" suele ser el primer paso al explorar GroupDocs.Redaction para Python a través de .NET. Sirve como una prueba simple para confirmar que su entorno de desarrollo está configurado correctamente y que la biblioteca funciona como se espera.

## Overview
GroupDocs.Redaction para Python a través de .NET le permite buscar, redactar y eliminar información sensible de varios formatos de documento. Una amplia gama de [formatos compatibles](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) lo hace versátil para diferentes casos de uso.

## How to redact a document
Los siguientes pasos demuestran cómo redactar información sensible de un documento usando GroupDocs.Redaction para Python a través de .NET:

1. Importe las clases `groupdocs.redaction` que necesite.
2. Describa la redacción (aquí, una frase exacta para reemplazar con un cuadro coloreado).
3. Instancie un [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) con la ruta al documento de ejemplo.
4. Aplique la redacción.
5. Guarde el resultado.

## Complete example
El ejemplo a continuación reemplaza cada aparición de la frase "John Doe" con un cuadro rojo semitransparente y guarda el documento redactado:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # Dibuje un cuadro rojo semitransparente sobre cada aparición de "John Doe"
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Cargue el documento, aplique la redacción y guarde el resultado
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

`sample.docx` es el archivo de ejemplo utilizado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) para descargarlo.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

Este ejemplo rasteriza el resultado a un PDF llamado `sample_redacted.pdf`, por lo que el contenido redactado no puede recuperarse (`save()` rasteriza a PDF por defecto; la opción `redacted_file_suffix` solo controla el nombre de salida). Para mantener el formato original, establezca `rasterize_to_pdf = False`.

## Additional resources
Esta demostración hace referencia a los [ejemplos de código](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/) de GroupDocs.Redaction para Python a través de .NET.
