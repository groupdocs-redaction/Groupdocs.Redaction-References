---
title: "Redactor-klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een hoofdklasse voor die het redactieproces van documenten regelt, waardoor documenten kunnen worden geopend, geredigeerd en opgeslagen."
type: docs
url: /nl/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Stelt een hoofdklasse voor die het redactieproces van documenten regelt, waardoor documenten kunnen worden geopend, geredigeerd en opgeslagen.

Meer informatie
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Het Redactor-type exposeert de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Initialiseert een nieuwe Redactor-instantie met een bestandspad. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Initialiseert een nieuwe instantie van [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) met een stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Initialiseert een nieuwe instantie van [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) voor een wachtwoord‑beveiligd document met het pad. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Initialiseert een nieuwe Redactor-instantie voor een wachtwoord‑beveiligd document met het pad en instellingen. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Initialiseert een nieuwe Redactor-instantie voor een wachtwoord‑beveiligd document met een stream. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Initialiseert een nieuwe instantie van [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) voor een wachtwoord‑beveiligd document met een stream en instellingen. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Past een redactie toe op het document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Past een reeks redacties toe op het document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Past een redactiebeleid toe op het document. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Vrijgeeft bronnen. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Genereert voorbeeldafbeeldingen van specifieke pagina's in een opgegeven afbeeldingsformaat. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Haalt de algemene informatie over het document op, zoals grootte en paginatelling. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Slaat het document op in een bestand met de volgende opties: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Slaat het document op in een bestand. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Slaat het document op in een stream, inclusief aangepaste locatie. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Open een document en verwijder de eerste pagina
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Taakgidsen die `Redactor` gebruiken:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### Zie ook
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
