---
title: "RedactionPolicy Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Bereinigungspolitik dar, die einen Satz spezifischer Redaktionen enthält, die angewendet werden sollen."
type: docs
url: /de/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Stellt eine Bereinigungspolitik dar, die einen Satz spezifischer Redaktionen enthält, die angewendet werden sollen.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

Der RedactionPolicy-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Initialisiert eine neue RedactionPolicy-Instanz. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Initialisiert eine neue RedactionPolicy mit einer spezifischen Liste von Redaktionen. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Lädt eine RedactionPolicy aus einer XML-Datei. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | Lädt eine RedactionPolicy-Instanz aus einem Stream, der XML-Konfiguration enthält. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Speichert die Redaktionsrichtlinie in einer Datei. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Speichert die Redaktionsrichtlinie in einen Stream. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | Die Liste der vollständig konfigurierten von [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)-abgeleiteten Klassen. |

### Beispiel

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Erstelle eine wiederverwendbare Richtlinie im Speicher
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Wende die Richtlinie auf ein Dokument an
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
Aufgabenleitfäden, die `RedactionPolicy` verwenden:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Siehe auch
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
