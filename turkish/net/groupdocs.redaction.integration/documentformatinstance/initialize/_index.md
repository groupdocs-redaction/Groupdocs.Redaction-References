---
title: "Initialize"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belge formatı işleyicisinin örneğinin başlatılmasını gerçekleştirir."
type: docs
weight: 20
url: /tr/net/groupdocs.redaction.integration/documentformatinstance/initialize/
---
## DocumentFormatInstance.Initialize method

Belge formatı işleyicisinin örneğinin başlatılmasını gerçekleştirir.

```csharp
public virtual void Initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| config | DocumentFormatConfiguration | Biçim yapılandırması |
| settings | RedactorSettings | Kırpma işlemi için varsayılan ayarlar. |

### Örnekler

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

* class [DocumentFormatConfiguration](../../../groupdocs.redaction.configuration/documentformatconfiguration)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [DocumentFormatInstance](../../documentformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
