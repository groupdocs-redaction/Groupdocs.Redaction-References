---
title: "GeneratePreview"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belirli sayfaların önizleme görüntülerini verilen bir görüntü formatında oluşturur."
type: docs
weight: 40
url: /tr/net/groupdocs.redaction/redactor/generatepreview/
---
## Redactor.GeneratePreview method

Belirli sayfaların önizleme görüntülerini verilen bir görüntü formatında oluşturur.

```csharp
public void GeneratePreview(PreviewOptions previewOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| previewOptions | PreviewOptions | Görüntü özellikleri ve sayfa aralığı ayarları |

### Örnekler

Aşağıdaki örnek, [`PreviewOptions`](../../../groupdocs.redaction.options/previewoptions) ve her iki temsilciyi kullanarak bir belge önizlemesinin nasıl alınacağını gösterir.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // Sayfa önizlemesi içeren Stream ile herhangi bir şey yapın
        pageStream.Close();
    };
    var previewOptions = new PreviewOptions(createDelegate, releaseDelegate);
    previewOptions.PreviewFormat = PreviewOptions.PreviewFormats.PNG;
    previewOptions.Height = 640;
    previewOptions.Width = 480;
    previewOptions.PageNumbers = new int[] { 1 };
    using (var redactor = new Redactor("C:\Temp\SourceFile.pdf"))
    {
        redactor.GeneratePreview(previewOptions);
    }
```

### Ayrıca Bakınız

* class [PreviewOptions](../../../groupdocs.redaction.options/previewoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
