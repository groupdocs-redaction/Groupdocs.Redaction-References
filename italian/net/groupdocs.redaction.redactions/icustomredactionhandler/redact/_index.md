---
title: "Redigi"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Applica una redazione personalizzata al contenuto specifico del documento. Attualmente è supportata solo per PDF PageAreaRedactiongroupdocs.redaction.redactions/pagearearedaction. Gli utenti possono definire la propria logica di redazione, come la redazione AIbased, che può essere più avanzata rispetto ai metodi patternbased semplici."
type: docs
weight: 10
url: /it/net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
---
## ICustomRedactionHandler.Redact method

Applica una redazione personalizzata al contenuto specifico del documento. Attualmente, è supportata solo per PDF [`PageAreaRedaction`](../../pagearearedaction). Gli utenti possono definire la propria logica di redazione, come la redazione AI-based, che può essere più avanzata rispetto ai metodi pattern-based semplici.

```csharp
public CustomRedactionResult Redact(CustomRedactionContext context)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| contesto | CustomRedactionContext | Contiene il contenuto del documento da redigere insieme ai metadati correlati. |

### Valore di ritorno

Un [`CustomRedactionResult`](../../customredactionresult) che indica se la redazione deve essere applicata e il contenuto modificato.

### Vedi anche

* class [CustomRedactionResult](../../customredactionresult)
* class [CustomRedactionContext](../../customredactioncontext)
* interface [ICustomRedactionHandler](../../icustomredactionhandler)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
