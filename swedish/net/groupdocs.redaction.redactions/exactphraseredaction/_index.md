---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en textredigering som ersätter exakt fras i dokumentets text utan att ta hänsyn till skiftläge som standard."
type: docs
weight: 600
url: /sv/net/groupdocs.redaction.redactions/exactphraseredaction/
---
## ExactPhraseRedaction class

Representerar en textredigering som ersätter exakt fras i dokumentets text, skiftlägesokänslig som standard.

```csharp
public class ExactPhraseRedaction : TextRedaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ExactPhraseRedaction](exactphraseredaction#constructor_1)(string, ReplacementOptions) | Initierar en ny instans av ExactPhraseRedaction-klassen i läge utan skiftlägeskänslighet. |
| [ExactPhraseRedaction](exactphraseredaction#constructor)(string, bool, ReplacementOptions) | Initierar en ny instans av ExactPhraseRedaction-klassen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Hämtar [`ReplacementOptions`](../replacementoptions)-instansen, som specificerar typen av textersättning. |
| override [Description](../../groupdocs.redaction.redactions/exactphraseredaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [IsCaseSensitive](../../groupdocs.redaction.redactions/exactphraseredaction/iscasesensitive) { get; } | Hämtar ett värde som indikerar om sökningen är skiftlägeskänslig eller inte. |
| [IsRightToLeft](../../groupdocs.redaction.redactions/exactphraseredaction/isrighttoleft) { get; set; } | Hämtar eller anger ett värde som indikerar om denna text är från höger till vänster eller inte, falskt som standard. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Hämtar eller anger [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector)-implementeringen som krävs för att extrahera text från grafiskt innehåll. |
| [SearchPhrase](../../groupdocs.redaction.redactions/exactphraseredaction/searchphrase) { get; } | Hämtar strängen som ska sökas och ersättas. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/exactphraseredaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Exempel

Följande exempel visar hur man utför en skiftlägeskänslig frassökning och ersättning.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Som standard är isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", true /*isCaseSensitive*/, new ReplacementOptions("[personal]")));
  doc.Save();
}
```

Följande exempel visar hur man ersätter en fras (utan skiftlägeskänslighet) med en solid röd rektangel.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Som standard är isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)));
  doc.Save();
}
```

### Se även

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
