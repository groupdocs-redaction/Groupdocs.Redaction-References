---
title: "RemovePages"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Supprime une ou plusieurs pages en fonction de son décalage de position de départ et du nombre."
type: docs
weight: 10
url: /fr/net/groupdocs.redaction.integration/ipaginateddocument/removepages/
---
## IPaginatedDocument.RemovePages method

Supprime une ou plusieurs pages en fonction de leur position de départ, du décalage et du nombre.

```csharp
public RedactionResult RemovePages(PageSeekOrigin origin, int index, int count)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| origine | PageSeekOrigin | Rechercher la position d'origine, le début ou la fin du document |
| indice | Int32 | Indice de position de départ (basé sur 0) |
| nombre | Int32 | Nombre de pages à supprimer |

### Valeur de retour

Résultat de la rédaction de la suppression des pages

### Voir aussi

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* enum [PageSeekOrigin](../../../groupdocs.redaction.redactions/pageseekorigin)
* interface [IPaginatedDocument](../../ipaginateddocument)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
