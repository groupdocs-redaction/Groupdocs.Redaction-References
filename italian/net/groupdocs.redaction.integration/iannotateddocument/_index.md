---
title: "IAnnotatedDocument"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Definisce i metodi necessari per l'accesso alle annotazioni, come i commenti. Deve essere implementato dalla classe DocumentFormatInstance./documentformatinstancederived per eseguire le redazioni delle annotazioni."
type: docs
weight: 120
url: /it/net/groupdocs.redaction.integration/iannotateddocument/
---
## IAnnotatedDocument interface

Definisce i metodi necessari per l'accesso alle annotazioni, come i commenti. Deve essere implementato dalla classe derivata da [`DocumentFormatInstance`](../documentformatinstance) per eseguire le redazioni delle annotazioni.

```csharp
public interface IAnnotatedDocument
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [DeleteAnnotations](../../groupdocs.redaction.integration/iannotateddocument/deleteannotations)(Regex) | Elimina tutte le annotazioni che corrispondono a un'espressione regolare nel documento. |
| [RedactAnnotation](../../groupdocs.redaction.integration/iannotateddocument/redactannotation)(Regex, string) | Sostituisce il testo corrispondente in tutte le annotazioni all'interno del documento. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Vedi anche

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
