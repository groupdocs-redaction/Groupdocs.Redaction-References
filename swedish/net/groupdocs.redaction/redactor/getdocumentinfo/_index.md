---
title: GetDocumentInfo
second_title: GroupDocs.Redaction för .NET API-referens
description: Får allmän information om dokumentet  storlek sidantal etc.
type: docs
weight: 50
url: /sv/net/groupdocs.redaction/redactor/getdocumentinfo/
---
## Redactor.GetDocumentInfo method

Får allmän information om dokumentet - storlek, sidantal, etc.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Returvärde

En instans av IDocumentInfo

### Exempel

Följande exempel visar hur man hämtar den allmänna dokumentinformationen med hjälp av[`IDocumentInfo`](../../idocumentinfo).

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

### Se även

* interface [IDocumentInfo](../../idocumentinfo)
* class [Redactor](../../redactor)
* namnutrymme [GroupDocs.Redaction](../../redactor)
* hopsättning [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->