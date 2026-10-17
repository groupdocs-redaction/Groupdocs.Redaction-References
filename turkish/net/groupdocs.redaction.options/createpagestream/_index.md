---
title: "CreatePageStream"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Sayfa önizleme verilerini yazmak için bir akış döndüren yöntemi temsil eder."
type: docs
weight: 300
url: /tr/net/groupdocs.redaction.options/createpagestream/
---
## CreatePageStream delegate

Sayfa önizleme verilerini yazmak için bir akış döndüren yöntemi temsil eder.

```csharp
public delegate Stream CreatePageStream(int pageNumber);
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageNumber | Int32 | Küçük resim oluşturulacak sayfanın sayfa numarası |

### Dönüş Değeri

Sayfa önizlemesini yazmak için akış

### Örnekler

Aşağıdaki örnek, [`PreviewOptions`](../previewoptions) ve [`CreatePageStream`](../createpagestream) temsilcisi kullanarak bir belge önizlemesinin nasıl alınacağını gösterir.

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

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
