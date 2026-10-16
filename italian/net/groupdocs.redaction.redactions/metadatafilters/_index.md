---
title: "MetadataFilters"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta un elenco dei tipi più comuni di metadati del documento."
type: docs
weight: 640
url: /it/net/groupdocs.redaction.redactions/metadatafilters/
---
## MetadataFilters enumeration

Rappresenta un elenco dei tipi più comuni di metadati del documento.

```csharp
[Flags]
public enum MetadataFilters
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Impostazione filtro vuoto, non corrisponde a nessun elemento di metadati. |
| Author | `1` | Autore del documento. |
| Category | `2` | Categoria del documento. |
| Comments | `4` | Commento per il documento. |
| Company | `8` | Azienda dell'Autore. |
| ContentStatus | `10` | Stato del contenuto. |
| CreatedTime | `20` | Data di creazione. |
| HyperlinkBase | `40` | Base del collegamento ipertestuale. |
| LastPrinted | `80` | Data e ora dell'ultima stampa. |
| LastSavedBy | `100` | Ultimo salvataggio da parte dell'utente. |
| LastSavedTime | `400` | Data e ora dell'ultimo salvataggio. |
| NameOfApplication | `800` | Nome dell'applicazione in cui è stato creato il documento. |
| Manager | `1000` | Nome del responsabile dell'autore. |
| RevisionNumber | `2000` | Numero di revisione. |
| Subject | `4000` | Oggetto del documento. |
| Template | `8000` | Nome del modello del documento. |
| Title | `10000` | Titolo del documento. |
| TotalEditingTime | `20000` | Tempo totale di modifica. |
| Version | `40000` | Versione del documento. |
| Description | `80000` | Descrizione del documento. |
| Keywords | `100000` | Parole chiave del documento. |
| ContentType | `200000` | Tipo di contenuto. |
| All | `7FFFFFFF` | Tutti i tipi degli elementi di metadati. |

### Osservazioni

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Vedi anche

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
