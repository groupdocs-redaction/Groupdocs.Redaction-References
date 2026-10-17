---
title: "PageInfo"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Kısa bir sayfa bilgisini temsil eder."
type: docs
weight: 480
url: /tr/net/groupdocs.redaction/pageinfo/
---
## PageInfo class

Kısa bir sayfa bilgisini temsil eder.

```csharp
public class PageInfo
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PageInfo](pageinfo)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Height](../../groupdocs.redaction/pageinfo/height) { get; set; } | Sayfa yüksekliğini alır veya ayarlar. |
| [PageNumber](../../groupdocs.redaction/pageinfo/pagenumber) { get; set; } | Sayfa numarasını alır veya ayarlar. |
| [Width](../../groupdocs.redaction/pageinfo/width) { get; set; } | Sayfa genişliğini alır veya ayarlar. |

### Açıklamalar

**Learn more**

* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Örnekler

Aşağıdaki örnek, [`IDocumentInfo`](../idocumentinfo) kullanarak genel belge bilgilerini nasıl alacağını gösterir.

```csharp
    try
    {
        using (Redactor red = new Redactor(@"C:\Temp\testfile.doc"))
        {
            IDocumentInfo docInfo = red.GetDocumentInfo();
            Console.WriteLine("Document size: {0}", docInfo.Size);
            Console.WriteLine("Document format: {0}", docInfo.FileType.FileFormat);
            Console.WriteLine("Document contains {0} pages", docInfo.PageCount);
            foreach (PageInfo page in docInfo.Pages)
            {
                Console.WriteLine("Page {0} size is {1}x{2}", page.PageNumber, page.Width, page.Height);
            }
        }
    }
    catch (GroupDocs.Redaction.Exceptions.PasswordRequiredException)
    {
        Console.WriteLine("You are trying to access document which is password protected. Please, set the password.");
    }
    catch (GroupDocs.Redaction.Exceptions.IncorrectPasswordException)
    {
        Console.WriteLine("The provided password is not valid.");
    }
```

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
