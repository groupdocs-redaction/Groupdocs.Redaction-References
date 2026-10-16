---
title: "IRedactionCallback"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Definisce i metodi richiesti per ricevere informazioni su ogni modifica di redazione e, facoltativamente, impedirla."
type: docs
weight: 620
url: /it/net/groupdocs.redaction.redactions/iredactioncallback/
---
## IRedactionCallback interface

Definisce i metodi richiesti per ricevere informazioni su ogni modifica di redazione e, facoltativamente, impedirla.

```csharp
public interface IRedactionCallback
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AcceptRedaction](../../groupdocs.redaction.redactions/iredactioncallback/acceptredaction)(RedactionDescription) | Questa chiamata viene attivata subito prima di applicare qualsiasi redazione al documento e consente di registrarla o di vietarla. |

### Osservazioni

**Learn more**

* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Esempi

Il seguente esempio dimostra come implementare la registrazione dettagliata per il processo di redazione.

```csharp
public class RedactionDump : IRedactionCallback
{
    public RedactionDump()
    {
    }

    public bool AcceptRedaction(RedactionDescription description)
    {
        Console.Write("{0} redaction, {1} action, item {2}. ", description.RedactionType, description.ActionType, description.OriginalText);
        if (description.Replacement != null)
        {
            Console.Write("Text {0} is replaced with {1}. ", description.Replacement.OriginalText, description.Replacement.Replacement);
        }
        Console.WriteLine();
        // puoi restituire "false" qui per impedire una modifica specifica durante il processo di redazione
        return true;
    }
}

...

// Assegna un'istanza prima di usare Redactor
Redactor.RedactionCallback = new RedactionDump();
```

### Vedi anche

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
