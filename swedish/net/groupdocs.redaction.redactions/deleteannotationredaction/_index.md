---
title: "DeleteAnnotationRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en textredigering som tar bort annotationer om texten matchar det givna reguljära uttrycket och eventuellt tar bort alla annotationer."
type: docs
weight: 580
url: /sv/net/groupdocs.redaction.redactions/deleteannotationredaction/
---
## DeleteAnnotationRedaction class

Representerar en textradering som tar bort annoteringar om texten matchar ett givet reguljärt uttryck (valfritt tar bort alla annoteringar).

```csharp
public class DeleteAnnotationRedaction : Redaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor)() | Initierar en ny instans av klassen DeleteAnnotationRedaction med inställningar för att ta bort alla annotationer (matchar allt). |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_2)(Regex) | Initierar en ny instans av klassen DeleteAnnotationRedaction och tar bort annotationer som matchar det givna uttrycket. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_1)(string) | Initierar en ny instans av klassen DeleteAnnotationRedaction och tar bort annotationer som matchar det givna uttrycket. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/deleteannotationredaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [Expression](../../groupdocs.redaction.redactions/deleteannotationredaction/expression) { get; } | Hämtar det reguljära uttrycket att matcha. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/deleteannotationredaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Exempel

Följande exempel visar hur man tar bort alla annotationer som innehåller orden "use", "show" eller "describe" från dokumentet (och behåller övriga).

```csharp
using (Redactor redactor = new Redactor(@"D:\test.docx"))
{
   redactor.Apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
   redactor.Save()
}
```

### Se även

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
