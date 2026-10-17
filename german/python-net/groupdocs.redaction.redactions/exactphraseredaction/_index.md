---
title: "ExactPhraseRedaction Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Textredaktion dar, die eine exakte Phrase im Dokumenttext ersetzt, standardmäßig ohne Berücksichtigung der Groß‑ und Kleinschreibung."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Stellt eine Textredaktion dar, die eine exakte Phrase im Dokumenttext ersetzt, standardmäßig ohne Berücksichtigung der Groß‑ und Kleinschreibung.

Mehr erfahren:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

Der ExactPhraseRedaction-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Initialisiert eine neue Instanz von ExactPhraseRedaction im Modus ohne Groß-/Kleinschreibung. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Initialisiert eine neue ExactPhraseRedaction-Instanz. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | Die Beschreibung der Redaktion, die den Redaktionsnamen und Parameter enthält. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | Der Wert, der angibt, ob die Suche Groß-/Kleinschreibung beachtet. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | Das Textausrichtungs-Flag, das angibt, ob der Text von rechts nach links verläuft. Standardwert ist False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | Der zu suchende und ersetzende String. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Die [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) Instanz, die den Typ der Textersetzung angibt. (geerbt von [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Die IOcrConnector-Implementierung, die verwendet wird, um Text aus grafischen Inhalten zu extrahieren. (geerbt von [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # Groß-/Kleinschreibung-sensitiver Ersatz
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Aufgabenleitfäden, die `ExactPhraseRedaction` verwenden:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
