---
title: "Hej, världen!"
linkTitle: "Hello, World!"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Kom snabbt igång med GroupDocs.Redaction för Python via .NET genom att skapa och köra ett enkelt exempel."
type: docs
url: /sv/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
Ett "Hej, världen!"-exempel är ofta det första steget när du utforskar GroupDocs.Redaction för Python via .NET. Det fungerar som ett enkelt test för att bekräfta att din utvecklingsmiljö är korrekt konfigurerad och att biblioteket fungerar som förväntat.

## Overview
GroupDocs.Redaction för Python via .NET låter dig söka, radera och ta bort känslig information från olika dokumentformat. Ett brett utbud av [supported formats](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) gör det mångsidigt för olika användningsområden.

## How to redact a document
Följande steg visar hur du raderar känslig information från ett dokument med hjälp av GroupDocs.Redaction för Python via .NET:

1. Importera de `groupdocs.redaction`-klasser du behöver.
2. Beskriv rödaktionen (här, en exakt fras att ersätta med en färgad ruta).
3. Skapa en instans av [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) med sökvägen till exempel-dokumentet.
4. Tillämpa rödaktionen.
5. Spara resultatet.

## Complete example
Exemplet nedan ersätter varje förekomst av frasen "John Doe" med en halvt genomskinlig röd ruta och sparar det raderade dokumentet:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # Rita en halvt genomskinlig röd ruta över varje förekomst av "John Doe"
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Läs in dokumentet, tillämpa rödaktionen och spara resultatet
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

`sample.docx` är exempel-filen som används i detta exempel. Klicka [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) för att ladda ner den.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

Detta exempel rasteriserar resultatet till en PDF med namnet `sample_redacted.pdf`, så den raderade innehållet kan inte återställas (`save()` rasteriserar till PDF som standard; alternativet `redacted_file_suffix` styr bara utdatafilens namn). För att behålla originalformatet istället, sätt `rasterize_to_pdf = False`.

## Additional resources
Denna demo refererar till GroupDocs.Redaction för Python via .NET [code samples](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/).
