---
title: "MetadataSearchRedaction Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Metadaten-Redaktion dar, die Metadaten mithilfe regulärer Ausdrücke sucht und redigiert, wobei Schlüssel und/oder Werte übereinstimmen."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Stellt eine Metadaten-Redaktion dar, die Metadaten mithilfe regulärer Ausdrücke sucht und redigiert, wobei Schlüssel und/oder Werte übereinstimmen.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

Der Typ MetadataSearchRedaction stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Initialisiert eine neue Instanz der Klasse MetadataSearchRedaction und verwendet den Wert, um zu redigierende Elemente zu finden. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Initialisiert eine neue Instanz von MetadataSearchRedaction und verwendet den Elementnamen und den Wert, um zu redigierende Elemente zu finden. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Initialisiert eine neue Instanz der Klasse MetadataSearchRedaction und verwendet den Wert, um zu redigierende Elemente zu finden. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Initialisiert eine neue Instanz von MetadataSearchRedaction, wobei der Elementname und der Wert zum Abgleichen zu redigierender Elemente verwendet werden. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Wendet die Redaktion auf eine gegebene Formatinstanz an. (geerbt von [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (geerbt von [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | Die Beschreibung der Redaktion, die ihren Namen und Parameter enthält. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | Der reguläre Ausdruck zum Abgleichen des Namens (Schlüssels) eines Metadaten‑Elements. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | Der textuelle Ersetzungswert. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | Der reguläre Ausdruck zum Abgleichen des Werttexts eines Metadaten‑Elements. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Der Filter, der verwendet wird, um alle oder bestimmte Metadaten auszuwählen, wie z. B. Autor oder Unternehmen. (geerbt von [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Redigieren Sie jeden Metadatenwert, der dem Muster entspricht
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Aufgabenleitfäden, die `MetadataSearchRedaction` verwenden:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
