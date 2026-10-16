---
title: "RemovePages"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rimuove una o più pagine a seconda dell'offset della posizione iniziale e del conteggio."
type: docs
weight: 10
url: /it/net/groupdocs.redaction.integration/ipaginateddocument/removepages/
---
## IPaginatedDocument.RemovePages method

Rimuove una o più pagine in base alla posizione di inizio, all'offset e al conteggio.

```csharp
public RedactionResult RemovePages(PageSeekOrigin origin, int index, int count)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | PageSeekOrigin | Cerca la posizione di origine, l'inizio o la fine del documento |
| indice | Int32 | Indice della posizione iniziale (basato su zero) |
| conteggio | Int32 | Numero di pagine da rimuovere |

### Valore di ritorno

Risultato della redazione della rimozione delle pagine

### Vedi anche

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* enum [PageSeekOrigin](../../../groupdocs.redaction.redactions/pageseekorigin)
* interface [IPaginatedDocument](../../ipaginateddocument)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
