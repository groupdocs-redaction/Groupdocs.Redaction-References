---
title: "MetadataSearchRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en metadataredigering som söker och raderar metadata med hjälp av reguljära uttryck som matchar nycklar och/eller värden."
type: docs
weight: 660
url: /sv/net/groupdocs.redaction.redactions/metadatasearchredaction/
---
## MetadataSearchRedaction class

Representerar en metadata‑redigering som söker och raderar metadata med reguljära uttryck, och matchar nycklar och/eller värden.

```csharp
public class MetadataSearchRedaction : MetadataRedaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_2)(Regex, string) | Initierar en ny instans av MetadataSearchRedaction-klassen, med värde för att matcha raderade objekt. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor)(string, string) | Initierar en ny instans av MetadataSearchRedaction-klassen, med värde för att matcha raderade objekt. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_3)(Regex, string, Regex) | Initierar en ny instans av MetadataSearchRedaction-klassen, med objektnamn och värde för att matcha raderade objekt. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_1)(string, string, string) | Initierar en ny instans av MetadataSearchRedaction-klassen, med objektnamn och värde för att matcha raderade objekt. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/metadatasearchredaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Hämtar eller anger filtret som används för att välja all eller specifik metadata, till exempel Author eller Company. |
| [KeyExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/keyexpression) { get; } | Hämtar det reguljära uttrycket för att matcha namn (nyckel) på metadataobjektet. |
| [Replacement](../../groupdocs.redaction.redactions/metadatasearchredaction/replacement) { get; } | Hämtar det textuella ersättningsvärdet. |
| [ValueExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/valueexpression) { get; } | Hämtar det reguljära uttrycket för att matcha värdetexten på ett metadataobjekt. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Exempel

Följande exempel visar hur man söker och raderar viss text i specifik metadata.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   MetadataSearchRedaction redaction = new MetadataSearchRedaction("Company Ltd.", "--company--");
   // Om den inte är angiven gäller den för alla metadataobjekt
   redaction.Filter = MetadataFilters.Company;
   redactor.Apply(redaction);
   redactor.Save();
}
```

### Se även

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
