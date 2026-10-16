---
title: "MetadataRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una classe astratta di base per le redazioni dei metadati del documento."
type: docs
weight: 650
url: /it/net/groupdocs.redaction.redactions/metadataredaction/
---
## MetadataRedaction class

Rappresenta una classe astratta di base per le redazioni dei metadati del documento.

```csharp
public abstract class MetadataRedaction : Redaction
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Ottiene o imposta il filtro, utilizzato per selezionare tutti o specifici metadati, ad esempio Autore o Azienda. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Vedi anche

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
