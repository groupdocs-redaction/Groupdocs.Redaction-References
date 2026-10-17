---
title: "AnnotationRedaction‑Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Redaktion dar, die Anmerkungstext (Kommentare usw.) ersetzt, der einem angegebenen regulären Ausdruck entspricht."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

Stellt eine Redaktion dar, die Anmerkungstext (Kommentare usw.) ersetzt, der einem angegebenen regulären Ausdruck entspricht.

Mehr erfahren

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Der AnnotationRedaction-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | Initialisiert ein neues AnnotationRedaction mit einem Regex‑Muster und Ersatztext. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | Initialisiert eine neue Instanz von [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/). |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | Die Beschreibung der Redaction, die die Redaction und ihre Parameter beschreibt. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | Der reguläre Ausdruck zum Abgleichen. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | Der Textersatz für übereinstimmenden Text. |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
Aufgabenleitfäden, die `AnnotationRedaction` verwenden:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
