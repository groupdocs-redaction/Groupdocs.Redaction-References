---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt redactie-instellingen voor die het aanpassen van het redactieproces mogelijk maken."
type: docs
weight: 430
url: /nl/net/groupdocs.redaction.options/redactorsettings/
---
## RedactorSettings class

Stelt redactie-instellingen voor, waarmee het redactieproces kan worden aangepast.

```csharp
public class RedactorSettings
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RedactorSettings](redactorsettings#constructor)() | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse. |
| [RedactorSettings](redactorsettings#constructor_2)(ILogger) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een opgegeven ILogger‑instantie. |
| [RedactorSettings](redactorsettings#constructor_1)(IOcrConnector) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een opgegeven IOcrConnector‑instantie. |
| [RedactorSettings](redactorsettings#constructor_5)(IRedactionCallback) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met een opgegeven IRedactionCallback‑instantie. |
| [RedactorSettings](redactorsettings#constructor_3)(ILogger, IRedactionCallback) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met opgegeven ILogger‑ en IRedactionCallback‑instanties. |
| [RedactorSettings](redactorsettings#constructor_4)(ILogger, IRedactionCallback, IOcrConnector) | Initialiseert een nieuw exemplaar van de RedactorSettings-klasse met opgegeven ILogger‑, IRedactionCallback‑ en IOcrConnector‑instanties. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [Logger](../../groupdocs.redaction.options/redactorsettings/logger) { get; set; } | Haalt een instantie van een klasse op of stelt deze in, die [`ILogger`](../ilogger) implementeert en wordt gebruikt voor het loggen van gebeurtenissen en fouten. |
| [OcrConnector](../../groupdocs.redaction.options/redactorsettings/ocrconnector) { get; set; } | Haalt een instantie van een klasse op of stelt deze in, die de interface [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) implementeert. |
| [RedactionCallback](../../groupdocs.redaction.options/redactorsettings/redactioncallback) { get; set; } | Haalt een instantie van een klasse op of stelt deze in, die [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) implementeert. |

### Opmerkingen

**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Zie ook

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
