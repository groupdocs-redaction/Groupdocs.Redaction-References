---
title: LoadOptions
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Fornisce le opzioni che verranno utilizzate per aprire un file.
type: docs
weight: 300
url: /it/net/groupdocs.redaction.options/loadoptions/
---
## LoadOptions class

Fornisce le opzioni che verranno utilizzate per aprire un file.

```csharp
public class LoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Inizializza una nuova istanza della classe LoadOptions. |
| [LoadOptions](loadoptions#constructor_1)(string) | Inizializza una nuova istanza della classe LoadOptions con la password specificata. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Password](../../groupdocs.redaction.options/loadoptions/password) { get; set; } | Ottiene o imposta una password per i documenti protetti da password. |

### Osservazioni

**Scopri di più**

* [Caricamento documenti](https://docs.groupdocs.com/redaction/net/loading-documents/)
* [Carica da disco locale](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
* [Carica dal flusso](https://docs.groupdocs.com/redaction/net/load-from-stream/)
* [Carica documento protetto da password](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

### Esempi

L'esempio seguente mostra come aprire un documento protetto da password.

```csharp
LoadOptions loadOptions = new LoadOptions("mysecretpassword");
using (var redactor = new Redactor("PasswordProtected.pdf", loadOptions))
{
    // lavora con il documento
}
```

### Guarda anche

* spazio dei nomi [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assemblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->