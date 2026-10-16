---
title: "MetadataSearchRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione dei metadati che ricerca e redige i metadati usando espressioni regolari che corrispondono a chiavi e/o valori."
type: docs
weight: 660
url: /it/net/groupdocs.redaction.redactions/metadatasearchredaction/
---
## MetadataSearchRedaction class

Rappresenta una redazione dei metadati che ricerca e cancella i metadati usando espressioni regolari, corrispondendo chiavi e/o valori.

```csharp
public class MetadataSearchRedaction : MetadataRedaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_2)(Regex, string) | Inizializza una nuova istanza della classe MetadataSearchRedaction, usando il valore per corrispondere agli elementi redatti. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor)(string, string) | Inizializza una nuova istanza della classe MetadataSearchRedaction, usando il valore per corrispondere agli elementi redatti. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_3)(Regex, string, Regex) | Inizializza una nuova istanza della classe MetadataSearchRedaction, usando il nome dell'elemento e il valore per corrispondere agli elementi redatti. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_1)(string, string, string) | Inizializza una nuova istanza della classe MetadataSearchRedaction, usando il nome dell'elemento e il valore per corrispondere agli elementi redatti. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/metadatasearchredaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Ottiene o imposta il filtro, utilizzato per selezionare tutti o specifici metadati, ad esempio Autore o Azienda. |
| [KeyExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/keyexpression) { get; } | Ottiene l'espressione regolare per corrispondere al nome (chiave) dell'elemento di metadati. |
| [Replacement](../../groupdocs.redaction.redactions/metadatasearchredaction/replacement) { get; } | Ottiene il valore di sostituzione testuale. |
| [ValueExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/valueexpression) { get; } | Ottiene l'espressione regolare per corrispondere al testo del valore di un elemento di metadati. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Esempi

Il seguente esempio dimostra come cercare e redigere determinati testi in metadati specifici.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   MetadataSearchRedaction redaction = new MetadataSearchRedaction("Company Ltd.", "--company--");
   // Se non impostato, si applica a tutti gli elementi dei metadati
   redaction.Filter = MetadataFilters.Company;
   redactor.Apply(redaction);
   redactor.Save();
}
```

### Vedi anche

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
