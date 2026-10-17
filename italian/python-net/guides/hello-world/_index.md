---
title: "Ciao, Mondo!"
linkTitle: "Hello, World!"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Inizia rapidamente con GroupDocs.Redaction per Python via .NET creando ed eseguendo un semplice esempio."
type: docs
url: /it/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
Un esempio \"Hello, World!\" è spesso il primo passo quando si esplora GroupDocs.Redaction per Python via .NET. Serve come un semplice test per confermare che l'ambiente di sviluppo sia configurato correttamente e che la libreria funzioni come previsto.

## Overview
GroupDocs.Redaction per Python via .NET ti consente di cercare, redigere e rimuovere informazioni sensibili da vari formati di documento. Un'ampia gamma di [formati supportati](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) lo rende versatile per diversi casi d'uso.

## How to redact a document
I passaggi seguenti mostrano come redigere informazioni sensibili da un documento usando GroupDocs.Redaction per Python via .NET:

1. Importa le classi `groupdocs.redaction` di cui hai bisogno.
2. Descrivi la redazione (qui, una frase esatta da sostituire con una casella colorata).
3. Istanzia un [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) con il percorso al documento di esempio.
4. Applica la redazione.
5. Salva il risultato.

## Complete example
L'esempio seguente sostituisce ogni occorrenza della frase \"John Doe\" con una casella rossa semitrasparente e salva il documento redatto:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # Disegna una casella rossa semitrasparente su ogni occorrenza di \"John Doe\"
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Carica il documento, applica la redazione e salva il risultato
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

`sample.docx` è il file di esempio usato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) per scaricarlo.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

Questo esempio rasterizza il risultato in un PDF chiamato `sample_redacted.pdf`, quindi il contenuto redatto non può essere recuperato (`save()` rasterizza in PDF per impostazione predefinita; l'opzione `redacted_file_suffix` controlla solo il nome del file di output). Per mantenere il formato originale invece, imposta `rasterize_to_pdf = False`.

## Additional resources
Questa demo fa riferimento ai [esempi di codice](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/) di GroupDocs.Redaction per Python via .NET.
