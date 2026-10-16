---
title: "AcceptRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Questa chiamata viene attivata subito prima di applicare qualsiasi redazione al documento e consente di registrarla o di vietarla."
type: docs
weight: 10
url: /it/net/groupdocs.redaction.redactions/iredactioncallback/acceptredaction/
---
## IRedactionCallback.AcceptRedaction method

Questa chiamata viene attivata subito prima di applicare qualsiasi redazione al documento e consente di registrarla o di vietarla.

```csharp
public bool AcceptRedaction(RedactionDescription description)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| descrizione | RedactionDescription | Contiene informazioni sul tipo di corrispondenza specifico, criteri, testo e posizione |

### Valore di ritorno

Restituisce true per accettare o false per rifiutare la redazione della corrispondenza specifica

### Vedi anche

* class [RedactionDescription](../../redactiondescription)
* interface [IRedactionCallback](../../iredactioncallback)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
