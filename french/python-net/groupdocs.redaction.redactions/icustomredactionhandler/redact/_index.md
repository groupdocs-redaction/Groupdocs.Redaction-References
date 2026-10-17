---
title: "méthode redact"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Applique une censure personnalisée à un contenu de document spécifique."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Applique une censure personnalisée à un contenu de document spécifique.

Actuellement, cela est pris en charge uniquement pour PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Les utilisateurs peuvent définir leur propre logique de rédaction, comme la rédaction basée sur l'IA, qui peut être plus avancée que les méthodes simples basées sur des modèles.

```python
def redact(self, context):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| context | `CustomRedactionContext` | Contient le contenu du document à rédiger ainsi que les métadonnées associées. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### Voir aussi
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
