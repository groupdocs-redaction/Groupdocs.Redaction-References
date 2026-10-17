---
title: "Klasse PageAreaRedaction"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine komplexe textuelle Redaktion dar, die Text, Bilder und Anmerkungen in einem Bereich der Seite beeinflusst."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

Stellt eine komplexe textuelle Redaktion dar, die Text, Bilder und Anmerkungen in einem Bereich der Seite beeinflusst.

Mehr erfahren

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

Der Typ PageAreaRedaction stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | Initialisiert eine neue PageAreaRedaction-Instanz. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | Initialisiert eine neue PageAreaRedaction. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | Die RegionReplacementOptions-Optionen mit Farb- und Flächenparametern. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Die [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) Instanz, die den Typ der Textersetzung angibt. (geerbt von [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Die Beschreibung der Redaktion, die ihren Namen und ihre Parameter enthält. (geerbt von [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Die IOcrConnector-Implementierung, die verwendet wird, um Text aus grafischen Inhalten zu extrahieren. (geerbt von [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Das reguläre Ausdrucksmuster, das für das Matching verwendet wird. (geerbt von [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
