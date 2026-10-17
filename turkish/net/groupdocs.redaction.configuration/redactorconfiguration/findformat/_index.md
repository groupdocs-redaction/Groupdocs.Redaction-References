---
title: "FindFormat"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belirli bir dosya uzantısı için format yapılandırmalarını bulur."
type: docs
weight: 30
url: /tr/net/groupdocs.redaction.configuration/redactorconfiguration/findformat/
---
## RedactorConfiguration.FindFormat method

Belirli bir dosya uzantısı için format yapılandırmalarını bulur.

```csharp
public DocumentFormatConfiguration FindFormat(string fileExtension)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileExtension | String | Dosya uzantısı, format ".ext" şeklindedir |

### Dönüş Değeri

Bulunursa, [`DocumentFormatConfiguration`](../../documentformatconfiguration) örneği, aksi takdirde null.

### Örnekler

Aşağıdaki örnek, yerleşik veya özel kullanıcı format işleyicilerinin nasıl alınacağını gösterir.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Ayrıca Bakınız

* class [DocumentFormatConfiguration](../../documentformatconfiguration)
* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
