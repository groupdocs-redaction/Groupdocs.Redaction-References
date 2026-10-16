---
title: "PageAreaRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione testuale complessa che influisce su testo, immagini e annotazioni in un'area della pagina."
type: docs
weight: 680
url: /it/net/groupdocs.redaction.redactions/pagearearedaction/
---
## PageAreaRedaction class

Rappresenta una redazione testuale complessa che influisce su testo, immagini e annotazioni in un'area della pagina.

```csharp
public class PageAreaRedaction : RegexRedaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PageAreaRedaction](pagearearedaction#constructor)(Regex, ReplacementOptions) | Inizializza una nuova istanza della classe PageAreaRedaction. |
| [PageAreaRedaction](pagearearedaction#constructor_1)(Regex, ReplacementOptions, RegionReplacementOptions) | Inizializza una nuova istanza della classe PageAreaRedaction. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Restituisce l'istanza di [`ReplacementOptions`](../replacementoptions), specificando il tipo di sostituzione del testo. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [ImageOptions](../../groupdocs.redaction.redactions/pagearearedaction/imageoptions) { get; } | Restituisce le opzioni [`RegionReplacementOptions`](../regionreplacementoptions) con parametri di colore e area. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Ottiene o imposta l'implementazione di [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), necessaria per estrarre il testo dal contenuto grafico. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Ottiene l'espressione regolare da corrispondere. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/pagearearedaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

### Vedi anche

* class [RegexRedaction](../regexredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
