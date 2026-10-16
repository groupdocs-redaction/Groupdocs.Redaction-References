---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een enkele wijzigingsactie‑informatie voor die tijdens het redactieproces wordt uitgevoerd."
type: docs
weight: 720
url: /nl/net/groupdocs.redaction.redactions/redactiondescription/
---
## RedactionDescription class

Stelt een enkele wijzigingsactie‑informatie voor die tijdens het redactieproces wordt uitgevoerd.

```csharp
public class RedactionDescription
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RedactionDescription](redactiondescription#constructor_1)(RedactionType, RedactionActionType, string) | Initialiseert een nieuw exemplaar van de RedactionDescription-klasse zonder vervangingsinformatie. |
| [RedactionDescription](redactiondescription#constructor)(RedactionType, RedactionActionType, RegionReplacementOptions, string) | Initialiseert een nieuw exemplaar van de RedactionDescription-klasse met vervangingsinformatie voor een afbeeldingsgebied. |
| [RedactionDescription](redactiondescription#constructor_2)(RedactionType, RedactionActionType, string, TextReplacement) | Initialiseert een nieuw exemplaar van de RedactionDescription-klasse met vervangingsinformatie. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/redactiondescription/actiontype) { get; } | Haalt de redactiebewerking op: vervanging, opschoning of verwijdering. |
| [Details](../../groupdocs.redaction.redactions/redactiondescription/details) { get; set; } | Haalt optionele detailinformatie op of stelt deze in voor het te redigeren item. |
| [ImageAreaReplacement](../../groupdocs.redaction.redactions/redactiondescription/imageareareplacement) { get; } | Haalt de vervangingsinformatie op voor redacties van afbeeldingsgebieden, retourneert null voor tekstredacties. |
| [OriginalText](../../groupdocs.redaction.redactions/redactiondescription/originaltext) { get; } | Haalt de overeenkomende tekst op, indien een expressie is opgegeven. |
| [RedactionType](../../groupdocs.redaction.redactions/redactiondescription/redactiontype) { get; } | Haalt het type documentgegevens op – tekst, metadata of annotaties. |
| [Replacement](../../groupdocs.redaction.redactions/redactiondescription/replacement) { get; } | Haalt de vervangingsinformatie op, kan null zijn. |

### Opmerkingen

**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Zie ook

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
