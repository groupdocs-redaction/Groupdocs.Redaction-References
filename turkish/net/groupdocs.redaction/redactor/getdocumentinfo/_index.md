---
title: "GetDocumentInfo"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belge hakkında genel bilgileri alır; boyut, sayfa sayısı vb."
type: docs
weight: 50
url: /tr/net/groupdocs.redaction/redactor/getdocumentinfo/
---
## Redactor.GetDocumentInfo method

Belge hakkında genel bilgileri alır - boyut, sayfa sayısı vb.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Dönüş Değeri

IDocumentInfo örneği

### Örnekler

Aşağıdaki örnek, [`IDocumentInfo`](../../idocumentinfo) kullanarak genel belge bilgilerini nasıl alacağınızı gösterir.

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

* interface [IDocumentInfo](../../idocumentinfo)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
