---
title: "IAnnotatedDocument"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Definierar metoder som krävs för åtkomst till annotationer såsom kommentarer. Måste implementeras av DocumentFormatInstance./documentformatinstancederived klass för att utföra annoteringsredigeringar."
type: docs
weight: 120
url: /sv/net/groupdocs.redaction.integration/iannotateddocument/
---
## IAnnotatedDocument interface

Definierar metoder som krävs för åtkomst till annotationer, såsom kommentarer. Måste implementeras av [`DocumentFormatInstance`](../documentformatinstance)-derived klass för att utföra annoteringsredigeringar.

```csharp
public interface IAnnotatedDocument
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [DeleteAnnotations](../../groupdocs.redaction.integration/iannotateddocument/deleteannotations)(Regex) | Tar bort alla annotationer som matchar reguljärt uttryck i dokumentet. |
| [RedactAnnotation](../../groupdocs.redaction.integration/iannotateddocument/redactannotation)(Regex, string) | Ersätter den matchande texten i alla annotationer i dokumentet. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Se även

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
