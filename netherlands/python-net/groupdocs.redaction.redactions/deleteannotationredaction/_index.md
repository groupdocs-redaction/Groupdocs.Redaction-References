---
title: "DeleteAnnotationRedaction klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een tekstredactie voor die annotaties verwijdert als de tekst overeenkomt met een gegeven reguliere expressie (optioneel worden alle annotaties verwijderd)."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Stelt een tekstredactie voor die annotaties verwijdert als de tekst overeenkomt met een gegeven reguliere expressie (optioneel worden alle annotaties verwijderd).

Meer informatie

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

Het type DeleteAnnotationRedaction exposeert de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction‑klasse, met instellingen om alle annotaties te verwijderen (alles matchend). |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction‑klasse, waarbij annotaties worden verwijderd die overeenkomen met de opgegeven expressie. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction‑klasse, waarbij annotaties worden verwijderd die overeenkomen met de opgegeven expressie. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Past de redactie toe op een gegeven formaat‑instantie. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | De beschrijving van de redactie, met de naam van de redactie en parameters. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | De reguliere expressie om te matchen. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # Verwijder annotaties die het woord "internal" bevatten (niet‑hoofdlettergevoelig)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
Taakgidsen die `DeleteAnnotationRedaction` gebruiken:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
