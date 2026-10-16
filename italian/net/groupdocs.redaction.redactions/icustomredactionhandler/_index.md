---
title: "ICustomRedactionHandler"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Fornisce un'interfaccia per implementare una logica di redazione personalizzata."
type: docs
weight: 610
url: /it/net/groupdocs.redaction.redactions/icustomredactionhandler/
---
## ICustomRedactionHandler interface

Fornisce un'interfaccia per implementare una logica di redazione personalizzata.

```csharp
public interface ICustomRedactionHandler
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Redact](../../groupdocs.redaction.redactions/icustomredactionhandler/redact)(CustomRedactionContext) | Applica una redazione personalizzata al contenuto specifico del documento. Attualmente, è supportata solo per PDF [`PageAreaRedaction`](../pagearearedaction). Gli utenti possono definire la propria logica di redazione, come la redazione basata su IA, che può essere più avanzata rispetto ai semplici metodi basati su pattern. |

### Vedi anche

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
