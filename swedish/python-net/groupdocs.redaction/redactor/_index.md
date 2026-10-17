---
title: "Redactor-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar en huvudklass som styr dokumentredigeringsprocessen och möjliggör att öppna, redigera och spara dokument."
type: docs
url: /sv/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Representerar en huvudklass som styr dokumentredigeringsprocessen och möjliggör att öppna, redigera och spara dokument.

Läs mer
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Redactor-typen exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Initierar en ny Redactor-instans med en filsökväg. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Initierar en ny instans av [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) med en ström. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Initierar en ny instans av [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) för ett lösenordsskyddat dokument med dess sökväg. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Initierar en ny Redactor-instans för ett lösenordsskyddat dokument med dess sökväg och inställningar. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Initierar en ny Redactor-instans för ett lösenordsskyddat dokument med en ström. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Initierar en ny instans av [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) för ett lösenordsskyddat dokument med en ström och inställningar. |

### Metoder
| Metod | Beskrivning |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Tillämpar en maskering på dokumentet. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Tillämpar en uppsättning maskeringar på dokumentet. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Tillämpar en maskeringspolicy på dokumentet. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Frigör resurser. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Genererar förhandsgranskningsbilder av specifika sidor i ett givet bildformat. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Hämtar den allmänna informationen om dokumentet, såsom storlek och sidantal. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Sparar dokumentet till en fil med följande alternativ: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Sparar dokumentet till en fil. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Sparar dokumentet till en ström, inklusive anpassad plats. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Exempel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Öppna ett dokument och ta bort den första sidan
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Uppgiftsguider som använder `Redactor`:

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

### Se även
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
