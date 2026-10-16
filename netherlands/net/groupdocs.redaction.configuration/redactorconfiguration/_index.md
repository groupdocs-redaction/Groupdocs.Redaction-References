---
title: "RedactorConfiguration"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Biedt toegang tot een lijst met ondersteunde formaten, ingebouwde en aangepaste gebruikersformaten."
type: docs
weight: 20
url: /nl/net/groupdocs.redaction.configuration/redactorconfiguration/
---
## RedactorConfiguration class

Biedt toegang tot een lijst met ondersteunde formaten, ingebouwde en aangepaste gebruikersformaten.

```csharp
public class RedactorConfiguration
```

## Properties

| Naam | Beschrijving |
| --- | --- |
| [AvailableFormats](../../groupdocs.redaction.configuration/redactorconfiguration/availableformats) { get; } | Haalt een lijst op van herkende formaten, zie [`DocumentFormatConfiguration`](../documentformatconfiguration). |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [GetInstance](../../groupdocs.redaction.configuration/redactorconfiguration/getinstance)() | Biedt een singleton‑instantie met de standaardconfiguratie van ingebouwde formaten. |
| [FindFormat](../../groupdocs.redaction.configuration/redactorconfiguration/findformat)(string) | Vindt formaatconfiguraties voor een gegeven bestandsextensie. |

### Opmerkingen

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Voorbeelden

Het volgende voorbeeld toont hoe een aangepaste gebruikersformaat‑handler toe te voegen.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

Het volgende voorbeeld toont hoe ingebouwde of aangepaste gebruikersformaat‑handlers op te halen.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Zie ook

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
