---
title: "AnnotationRedaction‑klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een redactie voor die annotatietekst (commentaren, enz.) vervangt die overeenkomt met een gegeven reguliere expressie."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

Stelt een redactie voor die annotatietekst (commentaren, enz.) vervangt die overeenkomt met een gegeven reguliere expressie.

Meer informatie

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Het type AnnotationRedaction biedt de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | Initialiseert een nieuwe AnnotationRedaction met een regex-patroon en vervangende tekst. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | Initialiseert een nieuw exemplaar van [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/). |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | Past de redactie toe op een gegeven formaat‑instantie. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | De beschrijving van de redactie, die de redactie en de parameters beschrijft. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | De reguliere expressie om te matchen. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | De tekstvervanging voor overeenkomende tekst. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
Taakgidsen die `AnnotationRedaction` gebruiken:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
