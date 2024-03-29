---
title: CellColumnRedaction
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Représente une rédaction de texte qui remplace le texte dans une feuille de calcul CSV Excel etc..
type: docs
weight: 450
url: /fr/net/groupdocs.redaction.redactions/cellcolumnredaction/
---
## CellColumnRedaction class

Représente une rédaction de texte qui remplace le texte dans une feuille de calcul (CSV, Excel, etc.).

```csharp
public class CellColumnRedaction : TextRedaction
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [CellColumnRedaction](cellcolumnredaction)(CellFilter, Regex, ReplacementOptions) | Initialise une nouvelle instance de la classe CellColumnRedaction. |

## Propriétés

| Nom | La description |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Obtient le[`ReplacementOptions`](../replacementoptions) instance, en spécifiant le type de remplacement de texte. |
| override [Description](../../groupdocs.redaction.redactions/cellcolumnredaction/description) { get; } | Renvoie une chaîne décrivant la rédaction et ses paramètres. |
| [Filter](../../groupdocs.redaction.redactions/cellcolumnredaction/filter) { get; } | Obtient le filtre de colonne et de feuille de calcul. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Obtient ou définit le[`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) mise en œuvre, nécessaire pour extraire le texte du contenu graphique. |
| [Pattern](../../groupdocs.redaction.redactions/cellcolumnredaction/pattern) { get; } | Obtient l'expression régulière correspondant. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/cellcolumnredaction/applyto)(DocumentFormatInstance) | Applique la rédaction à une instance de format donnée. |

### Remarques

**Apprendre encore plus**

* Plus de détails sur l'application des caviardages : [Les bases de la rédaction](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Plus de détails sur les suppressions de feuilles de calcul : [Caviardages des feuilles de calcul](https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/)

### Exemples

L'exemple suivant illustre la suppression des e-mails d'utilisateurs d'une deuxième colonne sur la feuille de calcul "Clients" d'un document de feuille de calcul.

```csharp
using (Redactor redactor = new Redactor("D:\\Sales in September.xslx"))
{
   var filter = new CellFilter()
   {
       ColumnIndex = 1, // 2e colonne de base zéro
       WorkSheetName = "Customers"
   };
   var expression = new Regex("^\\w+([-+.']\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$");
   RedactorChangeLog changeLog = redactor.Apply(new CellColumnRedaction(filter, expression, new ReplacementOptions("[customer email]")));
   if (result.Status != RedactionStatus.Failed)
   {
      doc.Save(new SaveOptions() { AddSuffix = true });
   };
}
```

### Voir également

* class [TextRedaction](../textredaction)
* espace de noms [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* Assemblée [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
