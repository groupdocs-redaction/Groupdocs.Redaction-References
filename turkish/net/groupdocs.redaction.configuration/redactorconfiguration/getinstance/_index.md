---
title: "GetInstance"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Yerleşik formatların varsayılan yapılandırmasıyla bir singleton örnek sağlar."
type: docs
weight: 10
url: /tr/net/groupdocs.redaction.configuration/redactorconfiguration/getinstance/
---
## RedactorConfiguration.GetInstance method

Yerleşik formatların varsayılan yapılandırmasıyla bir tekil örnek sağlar.

```csharp
public static RedactorConfiguration GetInstance()
```

### Dönüş Değeri

Yapılandırma örneği

### Örnekler

Aşağıdaki örnek, özel bir format işleyicisinin nasıl ekleneceğini gösterir.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

### Ayrıca Bakınız

* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
