---
title: Initialize
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Melakukan inisialisasi instance document format handler.
type: docs
weight: 20
url: /id/net/groupdocs.redaction.integration/documentformatinstance/initialize/
---
## DocumentFormatInstance.Initialize method

Melakukan inisialisasi instance document format handler.

```csharp
public virtual void Initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| config | DocumentFormatConfiguration | Konfigurasi format |
| settings | RedactorSettings | Pengaturan default untuk proses redaksi. |

### Contoh

Contoh berikut menunjukkan cara menggunakan data inisialisasi.

```csharp
public class MyCustomHandler : DocumentFormatInstance
{
    private string MyProperty { get; set; }
    
    // Kode khusus lainnya 
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

// Memasukkan format khusus ke GroupDocs.Redaction
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Lihat juga

* class [DocumentFormatConfiguration](../../../groupdocs.redaction.configuration/documentformatconfiguration)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [DocumentFormatInstance](../../documentformatinstance)
* ruang nama [GroupDocs.Redaction.Integration](../../documentformatinstance)
* perakitan [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->