---
title: "DocumentFormatInstance"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Bir belgenin belirli bir formatını temsil eder. Kendi belge türlerinizi eklemek için bu sınıfı uygulayın."
type: docs
weight: 110
url: /tr/net/groupdocs.redaction.integration/documentformatinstance/
---
## DocumentFormatInstance class

Bir belgenin belirli bir formatını temsil eder. Kendi belge türlerinizi eklemek için bu sınıfı uygulayın.

```csharp
public abstract class DocumentFormatInstance
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Password](../../groupdocs.redaction.integration/documentformatinstance/password) { get; set; } | Parola korumalı belgeler için bir parolayı alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [Initialize](../../groupdocs.redaction.integration/documentformatinstance/initialize)(DocumentFormatConfiguration, RedactorSettings) | Belge formatı işleyicisinin örneğinin başlatılmasını gerçekleştirir. |
| [IsRedactionAccepted](../../groupdocs.redaction.integration/documentformatinstance/isredactionaccepted)(RedactionDescription) | Belirtilmişse, [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) uygulamasını kontrol eder ve çağırır. |
| virtual [Load](../../groupdocs.redaction.integration/documentformatinstance/load)(Stream) | Belgeyi bir akıştan yükler. |
| virtual [PerformBinaryCheck](../../groupdocs.redaction.integration/documentformatinstance/performbinarycheck)(Stream) | Verilen akışın, bu format örneği tarafından desteklenen bir belge içerip içermediğini kontrol eder. |
| abstract [Save](../../groupdocs.redaction.integration/documentformatinstance/save)(Stream) | Belgeyi bir akışa kaydeder. |

### Açıklamalar

**Learn more**

* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Örnekler

Aşağıdaki örnek, özel bir format işleyicisi için boş bir taslak oluşturmayı gösterir.

```csharp
public class DummyDocument : DocumentFormatInstance
{     
    public override void Load(Stream output)
    {
        // dosya içeriğini yükle
    }

    public override void Save(Stream output)
    {
        // dosyaya değişiklikleri kaydet;
    }
}
```

Aşağıdaki örnek, başlatma verilerinin nasıl kullanılacağını gösterir.

```csharp
public class MyCustomHandler : DocumentFormatInstance
{
    private string MyProperty { get; set; }
    
    // Diğer özel kod 
    ...

    public override void Initialize(DocumentFormatConfiguration config)
    {
        base.Initialize(config);
        if (config.InitializationData.ContainsKey("MyProperty"))
        {
            MyProperty = config.InitializationData["MyProperty"];
        }
    }
}

// Özel formatı GroupDocs.Redaction içine entegre etme
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
