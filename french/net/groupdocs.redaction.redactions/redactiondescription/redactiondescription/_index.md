---
title: "RedactionDescription"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Initialise une nouvelle instance de la classe RedactionDescription sans informations de remplacement."
type: docs
weight: 10
url: /fr/net/groupdocs.redaction.redactions/redactiondescription/redactiondescription/
---
## RedactionDescription(RedactionType, RedactionActionType, string) {#constructor_1}

Initialise une nouvelle instance de la classe RedactionDescription sans informations de remplacement.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| redactionType | RedactionType | Type de données à censurer |
| actionType | RedactionActionType | Action à effectuer sur ces données |
| originalText | String | Texte correspondant, commentaire ou corps d'annotation |

### Voir aussi

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, string, TextReplacement) {#constructor_2}

Initialise une nouvelle instance de la classe RedactionDescription avec des informations de remplacement.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText, TextReplacement replacement)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| redactionType | RedactionType | Type de données à censurer |
| actionType | RedactionActionType | Action à effectuer sur ces données |
| originalText | String | Texte correspondant, commentaire ou corps d'annotation |
| remplacement | TextReplacement | Texte de remplacement, texte correspondant et sa position dans la chaîne originale |

### Voir aussi

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [TextReplacement](../../textreplacement)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, RegionReplacementOptions, string) {#constructor}

Initialise une nouvelle instance de la classe RedactionDescription avec des informations de remplacement de zone d'image.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    RegionReplacementOptions imageAreaReplacement, string imageDetails)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| redactionType | RedactionType | Type de données à censurer |
| actionType | RedactionActionType | Action à effectuer sur ces données |
| imageAreaReplacement | RegionReplacementOptions | Informations de remplacement de zone d'image |
| imageDetails | String | Description textuelle de l'image, par défaut c'est String.Empty |

### Voir aussi

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RegionReplacementOptions](../../regionreplacementoptions)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
