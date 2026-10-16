---
title: "CellColumnRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een tekstredactie voor die tekst vervangt in spreadsheet‑documenten, CSV, Excel, enz.."
type: docs
weight: 540
url: /nl/net/groupdocs.redaction.redactions/cellcolumnredaction/
---
## CellColumnRedaction class

Stelt een tekstredactie voor die tekst in spreadsheet‑documenten (CSV, Excel, enz.) vervangt.

```csharp
public class CellColumnRedaction : TextRedaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [CellColumnRedaction](cellcolumnredaction)(CellFilter, Regex, ReplacementOptions) | Initialiseert een nieuwe instantie van de klasse CellColumnRedaction. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Haalt de [`ReplacementOptions`](../replacementoptions) instantie op, die het type tekstvervanging specificeert. |
| override [Description](../../groupdocs.redaction.redactions/cellcolumnredaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [Filter](../../groupdocs.redaction.redactions/cellcolumnredaction/filter) { get; } | Haalt de kolom‑ en werkbladfilter op. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Haalt op of stelt de [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) implementatie in, die nodig is om tekst uit grafische inhoud te extraheren. |
| [Pattern](../../groupdocs.redaction.redactions/cellcolumnredaction/pattern) { get; } | Haalt de reguliere expressie op die moet overeenkomen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/cellcolumnredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about spreadsheet redactions: [Spreadsheet redactions](https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/)

### Voorbeelden

Het volgende voorbeeld toont het verwijderen van gebruikers‑e‑mailadressen uit een tweede kolom op het werkblad "Customers" van een spreadsheet‑document.

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

### Zie ook

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
