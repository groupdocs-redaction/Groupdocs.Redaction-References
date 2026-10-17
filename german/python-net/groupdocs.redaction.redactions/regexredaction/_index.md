---
title: "Klasse RegexRedaction"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Text-Redaktion dar, die Text im Dokument sucht und ersetzt, indem der bereitgestellte reguläre Ausdruck verwendet wird."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

Stellt eine Text-Redaktion dar, die Text im Dokument sucht und ersetzt, indem der bereitgestellte reguläre Ausdruck verwendet wird.

Mehr erfahren

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

Der Typ RegexRedaction stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | Initialisiert eine neue Instanz von RegexRedaction. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | Initialisiert eine neue RegexRedaction-Instanz. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Die Beschreibung der Redaktion, die ihren Namen und Parameter enthält. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Das für das Matching verwendete reguläre Ausdrucksmuster. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Die [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) Instanz, die den Typ der Textersetzung angibt. (geerbt von [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Die IOcrConnector-Implementierung, die verwendet wird, um Text aus grafischen Inhalten zu extrahieren. (geerbt von [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # mit Text ersetzen
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # mit blauem, solidem Rechteck ersetzen
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
Aufgabenleitfäden, die `RegexRedaction` verwenden:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
