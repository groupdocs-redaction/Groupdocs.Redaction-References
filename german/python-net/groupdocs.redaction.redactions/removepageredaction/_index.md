---
title: "RemovePageRedaction Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Redaktion dar, die eine Seite (Folie, Arbeitsblatt usw.) aus einem Dokument entfernt."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Stellt eine Redaktion dar, die eine Seite (Folie, Arbeitsblatt usw.) aus einem Dokument entfernt.

Mehr erfahren
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

Der RemovePageRedaction-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Initialisiert eine neue RemovePageRedaction. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | Die Anzahl der zu entfernenden Seiten. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | Der Startpositionsindex (0-basiert). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | Die Referenzposition für das Suchen, entweder der Anfang oder das Ende eines Dokuments. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | Die Beschreibung der Redaktion, die ihren Namen und Parameter enthält. (geerbt von [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Entferne 1 Seite, gezählt vom Ende des Dokuments
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(rem_opt)

        # Speichern Sie das redigierte Dokument
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
Aufgabenleitfäden, die `RemovePageRedaction` verwenden:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
