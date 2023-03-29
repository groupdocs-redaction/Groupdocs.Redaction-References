---
title: GetInstance
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Menyediakan instance tunggal dengan konfigurasi default format bawaan.
type: docs
weight: 10
url: /id/net/groupdocs.redaction.configuration/redactorconfiguration/getinstance/
---
## RedactorConfiguration.GetInstance method

Menyediakan instance tunggal dengan konfigurasi default format bawaan.

```csharp
public static RedactorConfiguration GetInstance()
```

### Nilai Pengembalian

Contoh konfigurasi

### Contoh

Contoh berikut menunjukkan cara menambahkan penangan format khusus.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

### Lihat juga

* class [RedactorConfiguration](../../redactorconfiguration)
* ruang nama [GroupDocs.Redaction.Configuration](../../redactorconfiguration)
* perakitan [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->