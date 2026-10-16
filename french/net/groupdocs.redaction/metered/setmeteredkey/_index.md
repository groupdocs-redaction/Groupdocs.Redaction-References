---
title: "SetMeteredKey"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Active le produit avec des clés Mesurées."
type: docs
weight: 20
url: /fr/net/groupdocs.redaction/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Active le produit avec des clés Mesurées.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| publicKey | String | La clé publique. |
| privateKey | String | La clé privée. |

### Exemples

L'exemple suivant montre comment activer le produit avec des clés Mesurées.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Voir aussi

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
