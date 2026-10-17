---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Önizleme oluşturma için gereksinimleri ve akış delegelerini ayarlamak için seçenekler sağlar."
type: docs
weight: 400
url: /tr/net/groupdocs.redaction.options/previewoptions/
---
## PreviewOptions class

Önizleme oluşturma için gereksinimleri ve akış delegelerini ayarlamak için seçenekler sağlar.

```csharp
public class PreviewOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | PreviewOptions sınıfının yeni bir örneğini başlatır, çıktı akışının kapanmasına neden olur. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | PreviewOptions sınıfının yeni bir örneğini başlatır, çıktı akışının daha sonraki kullanım için istemciye geri gönderilmesini sağlar. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CreatePageStream](../../groupdocs.redaction.options/previewoptions/createpagestream) { get; set; } | Sayfa akışı oluşturma temsilcisinin bir örneğini alır veya ayarlar. |
| [Height](../../groupdocs.redaction.options/previewoptions/height) { get; set; } | Sayfa önizleme yüksekliğini alır veya ayarlar. |
| [PageNumbers](../../groupdocs.redaction.options/previewoptions/pagenumbers) { get; set; } | Önizleme oluşturmak için sayfa numaralarının bir dizisini alır veya ayarlar. |
| [PreviewFormat](../../groupdocs.redaction.options/previewoptions/previewformat) { get; set; } | Önizleme görüntü formatını alır veya ayarlar. |
| [ReleasePageStream](../../groupdocs.redaction.options/previewoptions/releasepagestream) { get; set; } | Sayfa önizleme tamamlama temsilcisinin bir örneğini alır veya ayarlar. |
| [Width](../../groupdocs.redaction.options/previewoptions/width) { get; set; } | Sayfa önizleme genişliğini alır veya ayarlar. |

### Örnekler

Aşağıdaki örnek, [`PreviewOptions`](../previewoptions) ve [`CreatePageStream`](./createpagestream) temsilcisini kullanarak bir belge önizlemesinin nasıl alınacağını gösterir.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    var previewOptions = new PreviewOptions(createDelegate);
    previewOptions.PreviewFormat = PreviewOptions.PreviewFormats.PNG;
    previewOptions.Height = 640;
    previewOptions.Width = 480;
    previewOptions.PageNumbers = new int[] { 1 };
    using (var redactor = new Redactor("C:\Temp\SourceFile.pdf"))
    {
        redactor.GeneratePreview(previewOptions);
    }
```

Aşağıdaki örnek, [`PreviewOptions`](../previewoptions) ve her iki temsilciyi kullanarak bir belge önizlemesinin nasıl alınacağını gösterir.

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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
