---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Kırpma sürecini özelleştirmeye izin veren kırpma ayarlarını temsil eder."
type: docs
weight: 430
url: /tr/net/groupdocs.redaction.options/redactorsettings/
---
## RedactorSettings class

Redaksiyon ayarlarını temsil eder, redaksiyon sürecini özelleştirmeye olanak tanır.

```csharp
public class RedactorSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RedactorSettings](redactorsettings#constructor)() | RedactorSettings sınıfının yeni bir örneğini başlatır. |
| [RedactorSettings](redactorsettings#constructor_2)(ILogger) | Verilen bir ILogger örneğiyle RedactorSettings sınıfının yeni bir örneğini başlatır. |
| [RedactorSettings](redactorsettings#constructor_1)(IOcrConnector) | Verilen bir IOcrConnector örneğiyle RedactorSettings sınıfının yeni bir örneğini başlatır. |
| [RedactorSettings](redactorsettings#constructor_5)(IRedactionCallback) | Verilen bir IRedactionCallback örneğiyle RedactorSettings sınıfının yeni bir örneğini başlatır. |
| [RedactorSettings](redactorsettings#constructor_3)(ILogger, IRedactionCallback) | Verilen ILogger ve IRedactionCallback örnekleriyle RedactorSettings sınıfının yeni bir örneğini başlatır. |
| [RedactorSettings](redactorsettings#constructor_4)(ILogger, IRedactionCallback, IOcrConnector) | Verilen ILogger, IRedactionCallback ve IOcrConnector örnekleriyle RedactorSettings sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Logger](../../groupdocs.redaction.options/redactorsettings/logger) { get; set; } | Olayları ve hataları kaydetmek için kullanılan, [`ILogger`](../ilogger) arayüzünü uygulayan bir sınıf örneğini alır veya ayarlar. |
| [OcrConnector](../../groupdocs.redaction.options/redactorsettings/ocrconnector) { get; set; } | [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) arayüzünü uygulayan bir sınıf örneğini alır veya ayarlar. |
| [RedactionCallback](../../groupdocs.redaction.options/redactorsettings/redactioncallback) { get; set; } | [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) arayüzünü uygulayan bir sınıf örneğini alır veya ayarlar. |

### Açıklamalar

**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
