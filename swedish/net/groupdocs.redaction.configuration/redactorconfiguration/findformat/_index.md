---
title: "FindFormat"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Hittar formatkonfigurationer för en given filändelse."
type: docs
weight: 30
url: /sv/net/groupdocs.redaction.configuration/redactorconfiguration/findformat/
---
## RedactorConfiguration.FindFormat method

Hittar formatkonfigurationer för en given filändelse.

```csharp
public DocumentFormatConfiguration FindFormat(string fileExtension)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileExtension | String | Filändelse, formatet är ".ext" |

### Returvärde

Om den finns, en instans av [`DocumentFormatConfiguration`](../../documentformatconfiguration), annars null

### Exempel

Följande exempel visar hur man hämtar inbyggda eller anpassade användarformat‑hanterare.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Se även

* class [DocumentFormatConfiguration](../../documentformatconfiguration)
* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
