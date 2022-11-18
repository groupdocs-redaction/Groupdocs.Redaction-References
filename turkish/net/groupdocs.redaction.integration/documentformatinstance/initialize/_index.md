---
title: Initialize
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Belge biçimi işleyici örneğinin başlatılmasını gerçekleştirir.
type: docs
weight: 20
url: /tr/net/groupdocs.redaction.integration/documentformatinstance/initialize/
---
## DocumentFormatInstance.Initialize method

Belge biçimi işleyici örneğinin başlatılmasını gerçekleştirir.

```csharp
public virtual void Initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| config | DocumentFormatConfiguration | Biçim yapılandırması |
| settings | RedactorSettings | Düzeltme işlemi için varsayılan ayarlar. |

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

// Özel biçimi GroupDocs.Redaction'a ekleme
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Ayrıca bakınız

* class [DocumentFormatConfiguration](../../../groupdocs.redaction.configuration/documentformatconfiguration)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [DocumentFormatInstance](../../documentformatinstance)
* ad alanı [GroupDocs.Redaction.Integration](../../documentformatinstance)
* toplantı [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->