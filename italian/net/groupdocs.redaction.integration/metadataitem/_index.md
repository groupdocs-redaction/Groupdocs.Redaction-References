---
title: "MetadataItem"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta un elemento di metadati comune a tutti i formati supportati e utilizzato nelle redazioni dei metadati."
type: docs
weight: 220
url: /it/net/groupdocs.redaction.integration/metadataitem/
---
## MetadataItem class

Rappresenta un elemento di metadati, comune a tutti i formati supportati e utilizzato nelle redazioni di metadati.

```csharp
public class MetadataItem : ISerializable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MetadataItem](metadataitem)() | Inizializza una nuova istanza. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActualValue](../../groupdocs.redaction.integration/metadataitem/actualvalue) { get; } | Ottiene la rappresentazione stringa del valore dell'elemento di metadati. |
| [Category](../../groupdocs.redaction.integration/metadataitem/category) { get; set; } | Ottiene o imposta una categoria dell'elemento di metadati, ad esempio l'ID risorsa per un elemento di metadati di risorsa incorporata. |
| virtual [DictionaryKey](../../groupdocs.redaction.integration/metadataitem/dictionarykey) { get; } | Ottiene una chiave di dizionario per [`MetadataCollection`](../metadatacollection), utilizzando il suo OriginalName e altri dati. |
| [Filter](../../groupdocs.redaction.integration/metadataitem/filter) { get; set; } | Ottiene o imposta un valore di [`MetadataFilters`](../../groupdocs.redaction.redactions/metadatafilters), assegnato a questo elemento di metadati e utilizzato nella filtrazione degli elementi. |
| [IsCustom](../../groupdocs.redaction.integration/metadataitem/iscustom) { get; set; } | Ottiene o imposta un valore che indica se questo elemento è personalizzato (aggiunto dagli autori del documento). |
| [OriginalName](../../groupdocs.redaction.integration/metadataitem/originalname) { get; set; } | Ottiene o imposta il nome originale dell'elemento di metadati, così come appare nel documento. |
| [Values](../../groupdocs.redaction.integration/metadataitem/values) { get; set; } | Ottiene o imposta il valore dell'elemento di metadati. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [CreateClone](../../groupdocs.redaction.integration/metadataitem/createclone)() | Crea una clonazione profonda dell'istanza corrente. |
| virtual [GetObjectData](../../groupdocs.redaction.integration/metadataitem/getobjectdata)(SerializationInfo, StreamingContext) | Restituisce informazioni sulle proprietà serializzabili. |

### Vedi anche

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
