---
title: CreatePageStream
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Sayfa önizleme verilerini yazmak için bir akış döndüren yöntemi temsil eder.
type: docs
weight: 290
url: /tr/net/groupdocs.redaction.options/createpagestream/
---
## CreatePageStream delegate

Sayfa önizleme verilerini yazmak için bir akış döndüren yöntemi temsil eder.

```csharp
public delegate Stream CreatePageStream(int pageNumber);
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageNumber | Int32 | Küçük resim oluşturmak için bir sayfanın sayfa numarası |

### Geri dönüş değeri

Sayfa önizlemesini yazmak için akış

### Örnekler

Aşağıdaki örnek, kullanarak bir belge önizlemesinin nasıl alınacağını gösterir.[`PreviewOptions`](../previewoptions) Ve[`CreatePageStream`](../createpagestream) temsilci.

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

### Ayrıca bakınız

* ad alanı [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* toplantı [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
