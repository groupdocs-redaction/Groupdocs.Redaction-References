---
title: "GetInstance"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Biedt een singleton-instantie met de standaardconfiguratie van ingebouwde formaten."
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.configuration/redactorconfiguration/getinstance/
---
## RedactorConfiguration.GetInstance method

Biedt een singleton‑instantie met de standaardconfiguratie van ingebouwde formaten.

```csharp
public static RedactorConfiguration GetInstance()
```

### Retourwaarde

Configuratie-instantie

### Voorbeelden

Het volgende voorbeeld laat zien hoe een aangepaste formaat-handler toe te voegen.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

### Zie ook

* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
