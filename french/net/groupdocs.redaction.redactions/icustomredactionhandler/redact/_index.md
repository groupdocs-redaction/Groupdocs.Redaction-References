---
title: "Rédiger"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Applique une rédaction personnalisée au contenu spécifique du document. Actuellement, cela n'est pris en charge que pour le PDF PageAreaRedactiongroupdocs.redaction.redactions/pagearearedaction. Les utilisateurs peuvent définir leur propre logique de rédaction, telle que la rédaction basée sur l'IA, qui peut être plus avancée que les méthodes simples basées sur des modèles."
type: docs
weight: 10
url: /fr/net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
---
## ICustomRedactionHandler.Redact method

Applique une rédaction personnalisée au contenu spécifique du document. Actuellement, cela n'est pris en charge que pour le PDF [`PageAreaRedaction`](../../pagearearedaction). Les utilisateurs peuvent définir leur propre logique de rédaction, telle que la rédaction basée sur l'IA, qui peut être plus avancée que les méthodes simples basées sur des modèles.

```csharp
public CustomRedactionResult Redact(CustomRedactionContext context)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| contexte | CustomRedactionContext | Contient le contenu du document à rédiger ainsi que les métadonnées associées. |

### Valeur de retour

Un [`CustomRedactionResult`](../../customredactionresult) indiquant si la rédaction doit être appliquée et le contenu modifié.

### Voir aussi

* class [CustomRedactionResult](../../customredactionresult)
* class [CustomRedactionContext](../../customredactioncontext)
* interface [ICustomRedactionHandler](../../icustomredactionhandler)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
