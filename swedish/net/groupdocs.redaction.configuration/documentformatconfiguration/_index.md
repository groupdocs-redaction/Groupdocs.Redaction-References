---
title: "DocumentFormatConfiguration"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en typreferens för DocumentFormatInstance../groupdocs.redaction.integration/documentformatinstancederived‑klassen och en lista över stödjade filändelser för snabbare formatdetektering."
type: docs
weight: 10
url: /sv/net/groupdocs.redaction.configuration/documentformatconfiguration/
---
## DocumentFormatConfiguration class

Representerar en typreferens för [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance)-avledd klass och en lista över stödjade filändelser för snabbare formatdetektering.

```csharp
public class DocumentFormatConfiguration
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DocumentFormatConfiguration](documentformatconfiguration)() | Initierar en ny instans av DocumentFormatConfiguration‑klassen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DocumentType](../../groupdocs.redaction.configuration/documentformatconfiguration/documenttype) { get; set; } | Hämtar eller anger typen av en klass som ärver från [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |
| [ExtensionFilter](../../groupdocs.redaction.configuration/documentformatconfiguration/extensionfilter) { get; set; } | Hämtar eller anger en kommaseparerad (\",\") lista över filändelser (t.ex. \".pdf\"), skiftlägesokänslig. |
| [InitializationData](../../groupdocs.redaction.configuration/documentformatconfiguration/initializationdata) { get; set; } | Hämtar eller anger data som krävs för initiering av [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SupportsExtension](../../groupdocs.redaction.configuration/documentformatconfiguration/supportsextension)(string) | Kontrollerar om en given filändelse kan hanteras som DocumentType. |

### Anmärkningar

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Exempel

Följande exempel visar hur man sätter egenskaper för en anpassad formatkonfiguration.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
```

### Se även

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
