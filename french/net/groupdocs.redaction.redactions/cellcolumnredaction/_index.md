---
title: "CellColumnRedaction"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une rédaction de texte qui remplace le texte dans des documents de feuille de calcul, CSV, Excel, etc."
type: docs
weight: 540
url: /fr/net/groupdocs.redaction.redactions/cellcolumnredaction/
---
## CellColumnRedaction class

Représente une rédaction de texte qui remplace le texte dans des documents de feuille de calcul (CSV, Excel, etc.).

```csharp
public class CellColumnRedaction : TextRedaction
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CellColumnRedaction](cellcolumnredaction)(CellFilter, Regex, ReplacementOptions) | Initialise une nouvelle instance de la classe CellColumnRedaction. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Obtient l'instance [`ReplacementOptions`](../replacementoptions), spécifiant le type de remplacement de texte. |
| override [Description](../../groupdocs.redaction.redactions/cellcolumnredaction/description) { get; } | Renvoie une chaîne décrivant la redaction et ses paramètres. |
| [Filter](../../groupdocs.redaction.redactions/cellcolumnredaction/filter) { get; } | Obtient le filtre de colonne et de feuille de calcul. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Obtient ou définit l'implémentation [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), requise pour extraire le texte du contenu graphique. |
| [Pattern](../../groupdocs.redaction.redactions/cellcolumnredaction/pattern) { get; } | Obtient l'expression régulière à correspondre. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/cellcolumnredaction/applyto)(DocumentFormatInstance) | Applique la redaction à une instance de format donnée. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about spreadsheet redactions: [Spreadsheet redactions](https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/)

### Exemples

L'exemple suivant montre la suppression des e‑mails des utilisateurs d'une deuxième colonne de la feuille de calcul "Customers" d'un document de feuille de calcul.

```csharp
using (Redactor redactor = new Redactor("D:\\Sales in September.xslx"))
{
   var filter = new CellFilter()
   {
       ColumnIndex = 1, // zero-based 2nd column
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

### Voir aussi

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
