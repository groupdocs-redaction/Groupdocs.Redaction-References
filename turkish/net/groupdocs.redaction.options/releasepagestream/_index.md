---
title: "ReleasePageStream"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "CreatePageStream./createpagestream temsilcisi tarafından oluşturulan akışı serbest bırakan bir yöntemi temsil eder."
type: docs
weight: 440
url: /tr/net/groupdocs.redaction.options/releasepagestream/
---
## ReleasePageStream delegate

[`CreatePageStream`](../createpagestream) temsilcisi tarafından oluşturulan akışı serbest bırakan bir yöntemi temsil eder.

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageNumber | Int32 | Oluşturulan sayfa önizlemesinin sayfa numarası |
| pageStream | Akış | Oluşturulan sayfa önizlemesini içeren akış |

### Örnekler

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
