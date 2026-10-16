---
title: "FindFormat"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Vindt formaatconfiguraties voor een gegeven bestandsextensie."
type: docs
weight: 30
url: /nl/net/groupdocs.redaction.configuration/redactorconfiguration/findformat/
---
## RedactorConfiguration.FindFormat method

Vindt formaatconfiguraties voor een gegeven bestandsextensie.

```csharp
public DocumentFormatConfiguration FindFormat(string fileExtension)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileExtension | String | Bestandsextensie, formaat is \".ext\" |

### Retourwaarde

Indien gevonden, een instantie van [`DocumentFormatConfiguration`](../../documentformatconfiguration), anders null

### Voorbeelden

Het volgende voorbeeld toont hoe ingebouwde of aangepaste gebruikersformaat‑handlers op te halen.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Zie ook

* class [DocumentFormatConfiguration](../../documentformatconfiguration)
* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
