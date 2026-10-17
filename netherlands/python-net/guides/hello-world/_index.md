---
title: "Hallo, wereld!"
linkTitle: "Hello, World!"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Begin snel met GroupDocs.Redaction for Python via .NET door een eenvoudig voorbeeld te maken en uit te voeren."
type: docs
url: /nl/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
Een "Hello, World!"-voorbeeld is vaak de eerste stap bij het verkennen van GroupDocs.Redaction for Python via .NET. Het dient als een eenvoudige test om te bevestigen dat uw ontwikkelomgeving correct is ingesteld en dat de bibliotheek naar verwachting functioneert.

## Overview
GroupDocs.Redaction for Python via .NET stelt u in staat om te zoeken, te redigeren en gevoelige informatie te verwijderen uit verschillende documentformaten. Een breed scala aan [ondersteunde formaten](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) maakt het veelzijdig voor verschillende gebruikssituaties.

## How to redact a document
De volgende stappen laten zien hoe u gevoelige informatie uit een document kunt redigeren met GroupDocs.Redaction for Python via .NET:

1. Importeer de `groupdocs.redaction`-klassen die u nodig heeft.
2. Beschrijf de redactie (hier, een exacte zin die moet worden vervangen door een gekleurde rechthoek).
3. Instantieer een [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) met het pad naar het voorbeelddocument.
4. Pas de redactie toe.
5. Sla het resultaat op.

## Complete example
Het onderstaande voorbeeld vervangt elke keer dat de zin "John Doe" voorkomt door een halfdoorzichtige rode rechthoek en slaat het geredigeerde document op:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # Teken een halfdoorzichtige rode rechthoek over elke keer dat "John Doe" voorkomt
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Laad het document, pas de redactie toe en sla het resultaat op
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

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) om het te downloaden.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

Dit voorbeeld rastert het resultaat naar een PDF genaamd `sample_redacted.pdf`, zodat de geredigeerde inhoud niet kan worden hersteld (`save()` rastert standaard naar PDF; de optie `redacted_file_suffix` bepaalt alleen de uitvoernaam). Om in plaats daarvan het oorspronkelijke formaat te behouden, stel `rasterize_to_pdf = False` in.

## Additional resources
Deze demo verwijst naar de GroupDocs.Redaction for Python via .NET [codevoorbeelden](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/).
