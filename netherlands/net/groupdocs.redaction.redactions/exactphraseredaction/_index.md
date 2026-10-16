---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een tekstredactie voor die een exacte zin vervangt in de documenttekst, standaard hoofdletterongevoelig."
type: docs
weight: 600
url: /nl/net/groupdocs.redaction.redactions/exactphraseredaction/
---
## ExactPhraseRedaction class

Stelt een tekstredactie voor die exacte zinnen in de tekst van het document vervangt, standaard hoofdletterongevoelig.

```csharp
public class ExactPhraseRedaction : TextRedaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ExactPhraseRedaction](exactphraseredaction#constructor_1)(string, ReplacementOptions) | Initialiseert een nieuw exemplaar van de ExactPhraseRedaction-klasse in hoofdletterongevoelige modus. |
| [ExactPhraseRedaction](exactphraseredaction#constructor)(string, bool, ReplacementOptions) | Initialiseert een nieuw exemplaar van de ExactPhraseRedaction-klasse. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Haalt de [`ReplacementOptions`](../replacementoptions) instantie op, die het type tekstvervanging specificeert. |
| override [Description](../../groupdocs.redaction.redactions/exactphraseredaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [IsCaseSensitive](../../groupdocs.redaction.redactions/exactphraseredaction/iscasesensitive) { get; } | Haalt een waarde op die aangeeft of de zoekopdracht hoofdlettergevoelig is of niet. |
| [IsRightToLeft](../../groupdocs.redaction.redactions/exactphraseredaction/isrighttoleft) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of deze tekst right-to-Left is of niet, standaard false. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Haalt op of stelt de [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) implementatie in, die nodig is om tekst uit grafische inhoud te extraheren. |
| [SearchPhrase](../../groupdocs.redaction.redactions/exactphraseredaction/searchphrase) { get; } | Haalt de tekenreeks op die moet worden gezocht en vervangen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/exactphraseredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Voorbeelden

Het volgende voorbeeld toont het uitvoeren van een hoofdlettergevoelige zoek- en vervangactie voor een zin.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Standaard is isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", true /*isCaseSensitive*/, new ReplacementOptions("[personal]")));
  doc.Save();
}
```

Het volgende voorbeeld toont het vervangen van een zin (hoofdletterongevoelig) door een effen rode rechthoek.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Standaard is isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)));
  doc.Save();
}
```

### Zie ook

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
