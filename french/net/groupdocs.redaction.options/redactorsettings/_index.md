---
title: "RedactorSettings"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente les paramètres de rédaction permettant de personnaliser le processus de rédaction."
type: docs
weight: 430
url: /fr/net/groupdocs.redaction.options/redactorsettings/
---
## RedactorSettings class

Représente les paramètres de rédaction, permettant de personnaliser le processus de rédaction.

```csharp
public class RedactorSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RedactorSettings](redactorsettings#constructor)() | Initialise une nouvelle instance de la classe RedactorSettings. |
| [RedactorSettings](redactorsettings#constructor_2)(ILogger) | Initialise une nouvelle instance de la classe RedactorSettings avec une instance ILogger donnée. |
| [RedactorSettings](redactorsettings#constructor_1)(IOcrConnector) | Initialise une nouvelle instance de la classe RedactorSettings avec une instance IOcrConnector donnée. |
| [RedactorSettings](redactorsettings#constructor_5)(IRedactionCallback) | Initialise une nouvelle instance de la classe RedactorSettings avec une instance IRedactionCallback donnée. |
| [RedactorSettings](redactorsettings#constructor_3)(ILogger, IRedactionCallback) | Initialise une nouvelle instance de la classe RedactorSettings avec les instances ILogger et IRedactionCallback données. |
| [RedactorSettings](redactorsettings#constructor_4)(ILogger, IRedactionCallback, IOcrConnector) | Initialise une nouvelle instance de la classe RedactorSettings avec les instances ILogger, IRedactionCallback et IOcrConnector données. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Logger](../../groupdocs.redaction.options/redactorsettings/logger) { get; set; } | Obtient ou définit une instance d’une classe implémentant [`ILogger`](../ilogger), utilisée pour consigner les événements et les erreurs. |
| [OcrConnector](../../groupdocs.redaction.options/redactorsettings/ocrconnector) { get; set; } | Obtient ou définit une instance d’une classe implémentant l’interface [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector). |
| [RedactionCallback](../../groupdocs.redaction.options/redactorsettings/redactioncallback) { get; set; } | Obtient ou définit une instance d’une classe implémentant [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback). |

### Remarques

**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Voir aussi

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
