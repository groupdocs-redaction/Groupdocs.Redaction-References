---
title: "RedactorConfiguration"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Yerleşik ve özel kullanıcı formatlarından oluşan desteklenen formatların bir listesine erişim sağlar."
type: docs
weight: 20
url: /tr/net/groupdocs.redaction.configuration/redactorconfiguration/
---
## RedactorConfiguration class

Desteklenen formatların, yerleşik ve özel kullanıcı formatlarının bir listesine erişim sağlar.

```csharp
public class RedactorConfiguration
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AvailableFormats](../../groupdocs.redaction.configuration/redactorconfiguration/availableformats) { get; } | Tanımlanan formatların bir listesini alır, bakınız [`DocumentFormatConfiguration`](../documentformatconfiguration). |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [GetInstance](../../groupdocs.redaction.configuration/redactorconfiguration/getinstance)() | Yerleşik formatların varsayılan yapılandırmasıyla bir tekil örnek sağlar. |
| [FindFormat](../../groupdocs.redaction.configuration/redactorconfiguration/findformat)(string) | Belirli bir dosya uzantısı için format yapılandırmalarını bulur. |

### Açıklamalar

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Örnekler

Aşağıdaki örnek, özel bir kullanıcı format işleyicisinin nasıl ekleneceğini gösterir.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

Aşağıdaki örnek, yerleşik veya özel kullanıcı format işleyicilerinin nasıl alınacağını gösterir.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
