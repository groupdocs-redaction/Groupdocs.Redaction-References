---
title: "ReplaceInColumn"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Remplace toutes les correspondances par un remplacement donné dans la colonne et la feuille de calcul spécifiées."
type: docs
weight: 20
url: /fr/net/groupdocs.redaction.integration/icellularformatinstance/replaceincolumn/
---
## ReplaceInColumn(Regex, string, int, int) {#replaceincolumn_1}

Remplace toutes les correspondances par un remplacement donné dans la colonne et la feuille de calcul spécifiées.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column, 
    int sheet)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| regularExpression | Regex | Expression régulière pour rechercher et remplacer |
| remplacement | String | Remplacement textuel |
| colonne | Int32 | Indice de colonne basé sur zéro |
| feuille | Int32 | Index de feuille de calcul basé sur zéro |

### Valeur de retour

Résultat du remplacement

### Voir aussi

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

---

## ReplaceInColumn(Regex, string, int) {#replaceincolumn}

Remplace toutes les correspondances par un remplacement donné dans la colonne spécifiée sur toutes les feuilles de calcul.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| regularExpression | Regex | Expression régulière pour rechercher et remplacer |
| remplacement | String | Remplacement textuel |
| colonne | Int32 | Indice de colonne basé sur zéro |

### Valeur de retour

Résultat du remplacement

### Voir aussi

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
