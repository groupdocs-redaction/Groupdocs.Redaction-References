---
title: GetInstance
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Biedt een singletoninstantie met standaardconfiguratie van ingebouwde indelingen.
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.configuration/redactorconfiguration/getinstance/
---
## RedactorConfiguration.GetInstance method

Biedt een singleton-instantie met standaardconfiguratie van ingebouwde indelingen.

```csharp
public static RedactorConfiguration GetInstance()
```

### Winstwaarde

Configuratie-exemplaar

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een handler voor aangepaste indeling kunt toevoegen.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

### Zie ook

* class [RedactorConfiguration](../../redactorconfiguration)
* naamruimte [GroupDocs.Redaction.Configuration](../../redactorconfiguration)
* montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->