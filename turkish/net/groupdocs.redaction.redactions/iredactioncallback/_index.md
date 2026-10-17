---
title: "IRedactionCallback"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Her redaksiyon değişikliği hakkında bilgi almayı ve isteğe bağlı olarak engellemeyi gerektiren yöntemleri tanımlar."
type: docs
weight: 620
url: /tr/net/groupdocs.redaction.redactions/iredactioncallback/
---
## IRedactionCallback interface

Her redaksiyon değişikliği hakkında bilgi almayı ve isteğe bağlı olarak engellemeyi gerektiren yöntemleri tanımlar.

```csharp
public interface IRedactionCallback
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AcceptRedaction](../../groupdocs.redaction.redactions/iredactioncallback/acceptredaction)(RedactionDescription) | Bu çağrı, belgeye herhangi bir redaksiyon uygulanmadan hemen önce tetiklenir ve bunu kaydetmeye veya engellemeye olanak tanır. |

### Açıklamalar

**Learn more**

* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Örnekler

Aşağıdaki örnek, redaksiyon süreci için ayrıntılı günlük kaydı nasıl uygulanacağını gösterir.

```csharp
public class RedactionDump : IRedactionCallback
{
    public RedactionDump()
    {
    }

    public bool AcceptRedaction(RedactionDescription description)
    {
        Console.Write("{0} redaction, {1} action, item {2}. ", description.RedactionType, description.ActionType, description.OriginalText);
        if (description.Replacement != null)
        {
            Console.Write("Text {0} is replaced with {1}. ", description.Replacement.OriginalText, description.Replacement.Replacement);
        }
        Console.WriteLine();
        // Redaksiyon sürecinde belirli bir değişikliği önlemek için burada "false" döndürebilirsiniz.
        return true;
    }
}

...

// Redactor kullanmadan önce bir örnek atayın.
Redactor.RedactionCallback = new RedactionDump();
```

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
