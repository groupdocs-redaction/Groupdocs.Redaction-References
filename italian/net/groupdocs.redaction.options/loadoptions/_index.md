---
title: "LoadOptions"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Fornisce le opzioni che saranno utilizzate per aprire un file."
type: docs
weight: 380
url: /it/net/groupdocs.redaction.options/loadoptions/
---
## LoadOptions class

Fornisce le opzioni che saranno utilizzate per aprire un file.

```csharp
public class LoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Inizializza una nuova istanza della classe LoadOptions. |
| [LoadOptions](loadoptions#constructor_1)(bool) | Inizializza una nuova istanza della classe LoadOptions con il flag di prerasterizzazione specificato. |
| [LoadOptions](loadoptions#constructor_2)(FileType) | Inizializza una nuova istanza della classe LoadOptions con il tipo di file specificato. |
| [LoadOptions](loadoptions#constructor_3)(string) | Inizializza una nuova istanza della classe LoadOptions con la password specificata. |
| [LoadOptions](loadoptions#constructor_4)(string, bool) | Inizializza una nuova istanza della classe LoadOptions con la password specificata. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FileType](../../groupdocs.redaction.options/loadoptions/filetype) { get; set; } | Ottiene o imposta il tipo di file da aprire. |
| [Password](../../groupdocs.redaction.options/loadoptions/password) { get; set; } | Ottiene o imposta una password per i documenti protetti da password. |
| [PreRasterize](../../groupdocs.redaction.options/loadoptions/prerasterize) { get; set; } | Ottiene o imposta un valore che indica se il file deve essere prerasterizzato. |

### Osservazioni

**Learn more**

* [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
* [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
* [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
* [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

### Esempi

Il seguente esempio dimostra come aprire un documento protetto da password.

```csharp
LoadOptions loadOptions = new LoadOptions("mysecretpassword");
using (var redactor = new Redactor("PasswordProtected.pdf", loadOptions))
{
    // lavorare con il documento
}
```

### Vedi anche

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
