---
title: "AcceptRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Cet appel est déclenché juste avant l'application de toute rédaction au document et permet de l'enregistrer ou de l'interdire."
type: docs
weight: 10
url: /fr/net/groupdocs.redaction.redactions/iredactioncallback/acceptredaction/
---
## IRedactionCallback.AcceptRedaction method

Cet appel est déclenché juste avant l'application de toute rédaction au document et permet de l'enregistrer ou de l'interdire.

```csharp
public bool AcceptRedaction(RedactionDescription description)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| description | RedactionDescription | Contient des informations sur le type de correspondance particulier, les critères, le texte et la position |

### Valeur de retour

Renvoie true pour accepter ou false pour refuser la rédaction d'une correspondance particulière

### Voir aussi

* class [RedactionDescription](../../redactiondescription)
* interface [IRedactionCallback](../../iredactioncallback)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
