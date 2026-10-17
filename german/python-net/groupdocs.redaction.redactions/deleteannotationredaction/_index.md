---
title: "DeleteAnnotationRedaction Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Textredaktion dar, die Anmerkungen löscht, wenn der Text einem angegebenen regulären Ausdruck entspricht (optionalerweise werden alle Anmerkungen gelöscht)."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Stellt eine Textredaktion dar, die Anmerkungen löscht, wenn der Text einem angegebenen regulären Ausdruck entspricht (optionalerweise werden alle Anmerkungen gelöscht).

Mehr erfahren

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Der DeleteAnnotationRedaction-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | Initialisiert eine neue Instanz der DeleteAnnotationRedaction‑Klasse mit Einstellungen, um alle Anmerkungen zu löschen (alles passend). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | Initialisiert eine neue Instanz der DeleteAnnotationRedaction‑Klasse und löscht Anmerkungen, die dem angegebenen Ausdruck entsprechen. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | Initialisiert eine neue Instanz der DeleteAnnotationRedaction‑Klasse und löscht Anmerkungen, die dem angegebenen Ausdruck entsprechen. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | Die Beschreibung der Redaktion, die den Redaktionsnamen und Parameter enthält. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | Der reguläre Ausdruck zum Abgleichen. |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # Lösche Anmerkungen, die das Wort "internal" enthalten (Groß-/Kleinschreibung ignorierend)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
Aufgabenleitfäden, die `DeleteAnnotationRedaction` verwenden:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
