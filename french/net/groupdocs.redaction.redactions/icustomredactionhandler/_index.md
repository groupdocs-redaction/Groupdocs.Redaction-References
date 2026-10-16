---
title: "ICustomRedactionHandler"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Fournit une interface pour implémenter une logique de rédaction personnalisée."
type: docs
weight: 610
url: /fr/net/groupdocs.redaction.redactions/icustomredactionhandler/
---
## ICustomRedactionHandler interface

Fournit une interface pour implémenter une logique de rédaction personnalisée.

```csharp
public interface ICustomRedactionHandler
```

## Méthodes

| Nom | Description |
| --- | --- |
| [Redact](../../groupdocs.redaction.redactions/icustomredactionhandler/redact)(CustomRedactionContext) | Applique une rédaction personnalisée au contenu spécifique d'un document. Actuellement, cela n'est pris en charge que pour les PDF [`PageAreaRedaction`](../pagearearedaction). Les utilisateurs peuvent définir leur propre logique de rédaction, telle que la rédaction basée sur l'IA, qui peut être plus avancée que les méthodes simples basées sur des motifs. |

### Voir aussi

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
