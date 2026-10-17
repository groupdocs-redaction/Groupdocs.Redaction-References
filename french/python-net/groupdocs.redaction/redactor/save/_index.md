---
title: "méthode save"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Enregistre le document dans un fichier avec les options suivantes : AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /fr/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Enregistre le document dans un fichier avec les options suivantes : AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

Enregistre le document dans un fichier.

```python
def save(self, save_options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| save_options | `SaveOptions` | Options pour ajouter un suffixe ou rasteriser. |

**Returns:** Path to redacted document.

### Exemple

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Spécifiez les options de redaction
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer le masquage
        redactor.apply(ex_red)

        # Enregistrez le document redacté dans son format d'origine avec un suffixe de date
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

Enregistre le document dans un flux, y compris l'emplacement personnalisé.

```python
def save(self, document, rasterization_options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| document | `io.RawIOBase` | Flux cible. |
| rasterization_options | `RasterizationOptions` | Options pour rasteriser ou non et pour spécifier les pages à rasteriser. |

### Exemple

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # configurer la rasterisation pour ne traiter que la première diapositive
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # l'objet BytesIO contient maintenant le document enregistré
    data = stream.getvalue()
```

### Voir aussi
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
