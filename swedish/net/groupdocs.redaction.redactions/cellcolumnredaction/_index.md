---
title: "CellColumnRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en textredigering som ersätter text i ett kalkylblad, dokument, CSV, Excel etc."
type: docs
weight: 540
url: /sv/net/groupdocs.redaction.redactions/cellcolumnredaction/
---
## CellColumnRedaction class

Representerar en textradering som ersätter text i kalkylbladsdokument (CSV, Excel osv.).

```csharp
public class CellColumnRedaction : TextRedaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CellColumnRedaction](cellcolumnredaction)(CellFilter, Regex, ReplacementOptions) | Initierar en ny instans av klassen CellColumnRedaction. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Hämtar [`ReplacementOptions`](../replacementoptions)-instansen, som specificerar typen av textersättning. |
| override [Description](../../groupdocs.redaction.redactions/cellcolumnredaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [Filter](../../groupdocs.redaction.redactions/cellcolumnredaction/filter) { get; } | Hämtar kolumn- och arbetsbladsfiltret. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Hämtar eller anger [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector)-implementeringen som krävs för att extrahera text från grafiskt innehåll. |
| [Pattern](../../groupdocs.redaction.redactions/cellcolumnredaction/pattern) { get; } | Hämtar det reguljära uttrycket att matcha. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/cellcolumnredaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about spreadsheet redactions: [Spreadsheet redactions](https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/)

### Exempel

Följande exempel visar hur man tar bort användares e-postadresser från en andra kolumn i "Customers"-arbetsbladet i ett kalkylbladsdokument.

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

### Se även

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
