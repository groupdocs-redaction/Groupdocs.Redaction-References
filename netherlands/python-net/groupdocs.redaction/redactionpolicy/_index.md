---
title: "RedactionPolicy klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een sanitatiebeleid voor, dat een reeks specifieke redacties bevat die moeten worden toegepast."
type: docs
url: /nl/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Stelt een sanitatiebeleid voor, dat een reeks specifieke redacties bevat die moeten worden toegepast.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

Het RedactionPolicy-type geeft de volgende leden weer:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Initialiseert een nieuw RedactionPolicy‑object. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Initialiseert een nieuw RedactionPolicy met een specifieke lijst van redacties. |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Laadt een RedactionPolicy vanuit een XML‑bestand. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | Laadt een RedactionPolicy‑object vanuit een stream die XML‑configuratie bevat. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Slaat het redactiebeleid op in een bestand. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Slaat het redactiebeleid op in een stream. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | De lijst met volledig geconfigureerde [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)-afgeleide klassen. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Bouw een herbruikbaar beleid in het geheugen
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Pas het beleid toe op een document
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
Taakgidsen die `RedactionPolicy` gebruiken:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Zie ook
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
