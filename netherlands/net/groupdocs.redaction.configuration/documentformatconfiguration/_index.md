---
title: "DocumentFormatConfiguration"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een type‑referentie voor DocumentFormatInstance../groupdocs.redaction.integration/documentformatinstancederived class en ondersteunde bestandsextensielijst voor snellere formaterdetectie."
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.configuration/documentformatconfiguration/
---
## DocumentFormatConfiguration class

Stelt een type‑referentie voor [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance)-afgeleide klasse en ondersteunde bestandsextensielijst voor snellere formaterdetectie.

```csharp
public class DocumentFormatConfiguration
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [DocumentFormatConfiguration](documentformatconfiguration)() | Initialiseert een nieuwe instantie van de DocumentFormatConfiguration‑klasse. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [DocumentType](../../groupdocs.redaction.configuration/documentformatconfiguration/documenttype) { get; set; } | Haalt op of stelt het type van een klasse in, die erft van [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |
| [ExtensionFilter](../../groupdocs.redaction.configuration/documentformatconfiguration/extensionfilter) { get; set; } | Haalt op of stelt een door komma (\",\") gescheiden lijst van bestandsextensies in (bijvoorbeeld \".pdf\"), hoofdletterongevoelig. |
| [InitializationData](../../groupdocs.redaction.configuration/documentformatconfiguration/initializationdata) { get; set; } | Haalt op of stelt gegevens in, vereist voor de initialisatie van [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [SupportsExtension](../../groupdocs.redaction.configuration/documentformatconfiguration/supportsextension)(string) | Controleert of een gegeven bestandsextensie kan worden behandeld als DocumentType. |

### Opmerkingen

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Voorbeelden

Het volgende voorbeeld toont hoe eigenschappen in te stellen voor een aangepaste formaatconfiguratie.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
```

### Zie ook

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
