---
title: "Classe MetadataSearchRedaction"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta una redazione dei metadati che ricerca e oscura i metadati usando espressioni regolari, corrispondendo chiavi e/o valori."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Rappresenta una redazione dei metadati che ricerca e oscura i metadati usando espressioni regolari, corrispondendo chiavi e/o valori.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

Il tipo MetadataSearchRedaction espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | Inizializza una nuova istanza della classe MetadataSearchRedaction, utilizzando il valore per corrispondere agli elementi redatti. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | Inizializza una nuova istanza di MetadataSearchRedaction, utilizzando il nome e il valore dell'elemento per corrispondere agli elementi redatti. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | Inizializza una nuova istanza della classe MetadataSearchRedaction, utilizzando il valore per corrispondere agli elementi redatti. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | Inizializza una nuova istanza di MetadataSearchRedaction utilizzando il nome e il valore dell'elemento per corrispondere agli elementi redatti. |

### Metodi
| Metodo | Descrizione |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Applica la redazione a una determinata istanza di formato. (eredita da [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (eredita da [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | La descrizione della redazione, contenente il suo nome e i parametri. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | L'espressione regolare per corrispondere al nome (chiave) di un elemento di metadati. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | Il valore di sostituzione testuale. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | L'espressione regolare per corrispondere al testo del valore di un elemento di metadati. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Il filtro utilizzato per selezionare tutti o specifici metadati, come Autore o Azienda. (eredita da [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Esempio

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Redigi qualsiasi valore di metadati che corrisponde al modello
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
Guide operative che utilizzano `MetadataSearchRedaction`:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
