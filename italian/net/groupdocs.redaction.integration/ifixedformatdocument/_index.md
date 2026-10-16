---
title: "IFixedFormatDocument"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Definisce i metodi necessari per accedere a formati a struttura fissa, come PDF o presentazioni."
type: docs
weight: 140
url: /it/net/groupdocs.redaction.integration/ifixedformatdocument/
---
## IFixedFormatDocument interface

Definisce i metodi necessari per i formati di accesso a strutture fisse, come PDF o presentazioni.

```csharp
public interface IFixedFormatDocument
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [LoadImages](../../groupdocs.redaction.integration/ifixedformatdocument/loadimages)(RedactionFilter[]) | Carica un array di istanze di immagini raster contenute nel documento, corrispondenti al set [`RedactionFilter`](../../groupdocs.redaction.redactions/redactionfilter). |
| [RedactAnnotation](../../groupdocs.redaction.integration/ifixedformatdocument/redactannotation)(Regex, ReplacementOptions) | Sostituisce il testo corrispondente in tutte le annotazioni all'interno del documento con le opzioni specificate. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Vedi anche

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
