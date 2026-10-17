---
title: "DocumentFormatConfiguration"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Daha hızlı format algılaması için DocumentFormatInstance../groupdocs.redaction.integration/documentformatinstancederived sınıfı ve desteklenen dosya uzantıları listesi için bir tip referansını temsil eder."
type: docs
weight: 10
url: /tr/net/groupdocs.redaction.configuration/documentformatconfiguration/
---
## DocumentFormatConfiguration class

Daha hızlı format algılaması için [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance)-türetilmiş sınıf ve desteklenen dosya uzantıları listesi için bir tip referansını temsil eder.

```csharp
public class DocumentFormatConfiguration
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DocumentFormatConfiguration](documentformatconfiguration)() | DocumentFormatConfiguration sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DocumentType](../../groupdocs.redaction.configuration/documentformatconfiguration/documenttype) { get; set; } | [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) sınıfından türeten bir sınıfın tipini alır veya ayarlar. |
| [ExtensionFilter](../../groupdocs.redaction.configuration/documentformatconfiguration/extensionfilter) { get; set; } | Dosya uzantılarının (örneğin ".pdf") virgül (",") ile ayrılmış listesini alır veya ayarlar, büyük/küçük harfe duyarsız. |
| [InitializationData](../../groupdocs.redaction.configuration/documentformatconfiguration/initializationdata) { get; set; } | [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) başlatması için gerekli verileri alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SupportsExtension](../../groupdocs.redaction.configuration/documentformatconfiguration/supportsextension)(string) | Belirli bir dosya uzantısının DocumentType olarak işlenip işlenemeyeceğini kontrol eder. |

### Açıklamalar

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Örnekler

Aşağıdaki örnek, özel bir format yapılandırması için özelliklerin nasıl ayarlanacağını gösterir.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
```

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
