---
title: "redact-metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Tillämpar anpassad redigering på specifikt dokumentinnehåll."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Tillämpar anpassad redigering på specifikt dokumentinnehåll.

För närvarande stöds detta endast för PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Användare kan definiera sin egen maskeringslogik, såsom AI‑baserad maskering, som kan vara mer avancerad än enkla mönsterbaserade metoder.

```python
def redact(self, context):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| context | `CustomRedactionContext` | Innehåller dokumentinnehållet som ska maskeras tillsammans med relaterad metadata. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### Se även
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
