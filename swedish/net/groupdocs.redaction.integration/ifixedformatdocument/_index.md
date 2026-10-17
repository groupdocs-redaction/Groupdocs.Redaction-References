---
title: "IFixedFormatDocument"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Definierar metoder som krävs för åtkomst till format med fast struktur såsom PDF eller presentationer."
type: docs
weight: 140
url: /sv/net/groupdocs.redaction.integration/ifixedformatdocument/
---
## IFixedFormatDocument interface

Definierar metoder som krävs för åtkomstformat med fast struktur, såsom PDF eller presentationer.

```csharp
public interface IFixedFormatDocument
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [LoadImages](../../groupdocs.redaction.integration/ifixedformatdocument/loadimages)(RedactionFilter[]) | Läser in en array av rasterbildsinstanser som finns i dokumentet och matchar [`RedactionFilter`](../../groupdocs.redaction.redactions/redactionfilter)-uppsättningen. |
| [RedactAnnotation](../../groupdocs.redaction.integration/ifixedformatdocument/redactannotation)(Regex, ReplacementOptions) | Ersätter den matchande texten i alla annotationer i dokumentet med angivna alternativ. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Se även

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
