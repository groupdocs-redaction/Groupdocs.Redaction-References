---
title: "RedactorConfiguration"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tillhandahåller åtkomst till en lista över stödjade format, inbyggda och anpassade användarformat."
type: docs
weight: 20
url: /sv/net/groupdocs.redaction.configuration/redactorconfiguration/
---
## RedactorConfiguration class

Tillhandahåller åtkomst till en lista över stödjade format, inbyggda och anpassade användarformat.

```csharp
public class RedactorConfiguration
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AvailableFormats](../../groupdocs.redaction.configuration/redactorconfiguration/availableformats) { get; } | Hämtar en lista över igenkända format, se [`DocumentFormatConfiguration`](../documentformatconfiguration). |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [GetInstance](../../groupdocs.redaction.configuration/redactorconfiguration/getinstance)() | Tillhandahåller en singleton-instans med standardkonfiguration för inbyggda format. |
| [FindFormat](../../groupdocs.redaction.configuration/redactorconfiguration/findformat)(string) | Hittar formatkonfigurationer för en given filändelse. |

### Anmärkningar

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Exempel

Följande exempel visar hur man lägger till en anpassad användarformat‑hanterare.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

Följande exempel visar hur man hämtar inbyggda eller anpassade användarformat‑hanterare.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Se även

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
