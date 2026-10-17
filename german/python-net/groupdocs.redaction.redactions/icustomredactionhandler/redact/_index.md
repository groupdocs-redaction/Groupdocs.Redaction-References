---
title: "redact Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Wendet benutzerdefinierte Redaktion auf spezifischen Dokumentinhalt an."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Wendet benutzerdefinierte Redaktion auf spezifischen Dokumentinhalt an.

Derzeit wird dies nur für PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/) unterstützt.

Benutzer können ihre eigene Redaktionslogik definieren, z. B. KI-basierte Redaktion, die möglicherweise fortschrittlicher ist als einfache, musterbasierte Methoden.

```python
def redact(self, context):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| context | `CustomRedactionContext` | Enthält den zu redigierenden Dokumentinhalt zusammen mit zugehörigen Metadaten. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### Siehe auch
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
