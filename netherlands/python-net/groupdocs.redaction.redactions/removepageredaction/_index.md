---
title: "RemovePageRedaction klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een redactie voor die een pagina (dia, werkblad, enz.) uit een document verwijdert."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Stelt een redactie voor die een pagina (dia, werkblad, enz.) uit een document verwijdert.

Meer informatie
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

Het RemovePageRedaction type maakt de volgende leden beschikbaar:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Initialiseert een nieuwe RemovePageRedaction. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Past de redactie toe op een gegeven formaat‑instantie. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | Het aantal te verwijderen pagina's. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | De startpositie‑index (0-gebaseerd). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | De referentiepositie voor zoeken, ofwel het begin of het einde van een document. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | De beschrijving van de redactie, met de naam en parameters. (geërfd van [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Verwijder 1 pagina, geteld vanaf het einde van het document
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Pas de redactie toe
        result = redactor.apply(rem_opt)

        # Sla het geredigeerde document op
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Taakgidsen die `RemovePageRedaction` gebruiken:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
