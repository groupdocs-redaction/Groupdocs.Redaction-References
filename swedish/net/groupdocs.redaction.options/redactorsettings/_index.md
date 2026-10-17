---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar raderingsinställningar som möjliggör anpassning av raderingsprocessen."
type: docs
weight: 430
url: /sv/net/groupdocs.redaction.options/redactorsettings/
---
## RedactorSettings class

Representerar redigeringsinställningar som möjliggör anpassning av redigeringsprocessen.

```csharp
public class RedactorSettings
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RedactorSettings](redactorsettings#constructor)() | Initierar en ny instans av klassen RedactorSettings. |
| [RedactorSettings](redactorsettings#constructor_2)(ILogger) | Initierar en ny instans av klassen RedactorSettings med en given ILogger-instans. |
| [RedactorSettings](redactorsettings#constructor_1)(IOcrConnector) | Initierar en ny instans av klassen RedactorSettings med en given IOcrConnector-instans. |
| [RedactorSettings](redactorsettings#constructor_5)(IRedactionCallback) | Initierar en ny instans av klassen RedactorSettings med en given IRedactionCallback-instans. |
| [RedactorSettings](redactorsettings#constructor_3)(ILogger, IRedactionCallback) | Initierar en ny instans av klassen RedactorSettings med givna ILogger- och IRedactionCallback-instanser. |
| [RedactorSettings](redactorsettings#constructor_4)(ILogger, IRedactionCallback, IOcrConnector) | Initierar en ny instans av klassen RedactorSettings med givna ILogger-, IRedactionCallback- och IOcrConnector-instanser. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Logger](../../groupdocs.redaction.options/redactorsettings/logger) { get; set; } | Hämtar eller anger en instans av en klass som implementerar [`ILogger`](../ilogger) och som används för att logga händelser och fel. |
| [OcrConnector](../../groupdocs.redaction.options/redactorsettings/ocrconnector) { get; set; } | Hämtar eller anger en instans av en klass som implementerar gränssnittet [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector). |
| [RedactionCallback](../../groupdocs.redaction.options/redactorsettings/redactioncallback) { get; set; } | Hämtar eller anger en instans av en klass som implementerar [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback). |

### Anmärkningar

**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Se även

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
