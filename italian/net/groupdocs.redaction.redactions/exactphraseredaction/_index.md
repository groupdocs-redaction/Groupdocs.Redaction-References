---
title: "ExactPhraseRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione di testo che sostituisce la frase esatta nel testo del documento, senza distinzione tra maiuscole e minuscole per impostazione predefinita."
type: docs
weight: 600
url: /it/net/groupdocs.redaction.redactions/exactphraseredaction/
---
## ExactPhraseRedaction class

Rappresenta una redazione del testo che sostituisce la frase esatta nel testo del documento, senza distinzione tra maiuscole e minuscole per impostazione predefinita.

```csharp
public class ExactPhraseRedaction : TextRedaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ExactPhraseRedaction](exactphraseredaction#constructor_1)(string, ReplacementOptions) | Inizializza una nuova istanza della classe ExactPhraseRedaction in modalità senza distinzione tra maiuscole e minuscole. |
| [ExactPhraseRedaction](exactphraseredaction#constructor)(string, bool, ReplacementOptions) | Inizializza una nuova istanza della classe ExactPhraseRedaction. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Restituisce l'istanza di [`ReplacementOptions`](../replacementoptions), specificando il tipo di sostituzione del testo. |
| override [Description](../../groupdocs.redaction.redactions/exactphraseredaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [IsCaseSensitive](../../groupdocs.redaction.redactions/exactphraseredaction/iscasesensitive) { get; } | Restituisce un valore che indica se la ricerca è sensibile al maiuscolo o meno. |
| [IsRightToLeft](../../groupdocs.redaction.redactions/exactphraseredaction/isrighttoleft) { get; set; } | Ottiene o imposta un valore che indica se questo testo è da destra a sinistra o meno, false per impostazione predefinita. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Ottiene o imposta l'implementazione di [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), necessaria per estrarre il testo dal contenuto grafico. |
| [SearchPhrase](../../groupdocs.redaction.redactions/exactphraseredaction/searchphrase) { get; } | Ottiene la stringa da cercare e sostituire. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/exactphraseredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Esempi

Il seguente esempio dimostra l'esecuzione di una ricerca e sostituzione di frase sensibile al maiuscolo.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Per impostazione predefinita, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", true /*isCaseSensitive*/, new ReplacementOptions("[personal]")));
  doc.Save();
}
```

Il seguente esempio dimostra la sostituzione della frase (senza distinzione tra maiuscole e minuscole) con un rettangolo rosso solido.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Per impostazione predefinita, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)));
  doc.Save();
}
```

### Vedi anche

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
