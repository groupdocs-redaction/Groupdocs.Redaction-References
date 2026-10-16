---
title: "EraseMetadataRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione dei metadati che cancella tutti i metadati o i metadati corrispondenti a specifici MetadataFilters dal documento."
type: docs
weight: 590
url: /it/net/groupdocs.redaction.redactions/erasemetadataredaction/
---
## EraseMetadataRedaction class

Rappresenta una redazione dei metadati che cancella tutti i metadati o i metadati corrispondenti a specifici MetadataFilters dal documento.

```csharp
public class EraseMetadataRedaction : MetadataRedaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [EraseMetadataRedaction](erasemetadataredaction#constructor)() | Inizializza una nuova istanza della classe EraseMetadataRedaction, cancellando tutti i metadati. |
| [EraseMetadataRedaction](erasemetadataredaction#constructor_1)(MetadataFilters) | Inizializza una nuova istanza della classe EraseMetadataRedaction, cancellando i metadati, corrispondendo a una combinazione specifica di [`MetadataFilters`](../metadatafilters). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/erasemetadataredaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Ottiene o imposta il filtro, utilizzato per selezionare tutti o specifici metadati, ad esempio Autore o Azienda. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Esempi

Il seguente esempio dimostra come cancellare (impostare a valori vuoti) tutti o specifici metadati.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   // Cancella Autore, Manager e Azienda
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.Author | MetadataFilters.Manager | MetadataFilters.Company));
   // Cancella tutti i metadati
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.All));
   redactor.Save();
}
```

### Vedi anche

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
