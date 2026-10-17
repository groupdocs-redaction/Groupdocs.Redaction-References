---
title: "ReplacementOptions klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt opties voor het vervangen van gematchte tekst voor."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Stelt opties voor het vervangen van gematchte tekst voor.

Meer informatie

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

Het type ReplacementOptions geeft de volgende leden weer:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Initialiseert een nieuw exemplaar van ReplacementOptions met de opgegeven vervangende tekst. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Initialiseert een nieuw exemplaar van de klasse ReplacementOptions met een gekleurde rechthoek als optie. |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | De vervangingsactie: teken vak of vervang tekst. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | De kleur voor een `ReplacementType.draw_box`-optie (anders genegeerd). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | De aangepaste redactiehandler die gebruikers in staat stelt hun eigen redactie‑logica te definiëren. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | De array met filters die op deze redactie moeten worden toegepast. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | De tekstuele vervangingswaarde. |

### Voorbeeld

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Vervang overeenkomende tekst door de tijdelijke aanduiding \"[X]\"
repl_opt = ReplacementOptions("[X]")
```

### Guides
Taakgidsen die `ReplacementOptions` gebruiken:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Zie ook
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
