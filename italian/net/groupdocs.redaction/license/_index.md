---
title: "License"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Fornisce metodi per applicare la licenza."
type: docs
weight: 270
url: /it/net/groupdocs.redaction/license/
---
## License class

Fornisce metodi per applicare la licenza.

```csharp
public class License
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [License](license)() | Inizializza un'istanza della classe License. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense)(Stream) | Imposta la licenza di GroupDocs.Redaction da uno stream. |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense_1)(string) | Imposta la licenza di GroupDocs.Redaction da un percorso file. |

### Osservazioni

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Esempi

Il seguente esempio dimostra come impostare la licenza per GroupDocs.Redaction.

```csharp
GroupDocs.Redaction.License license = new GroupDocs.Redaction.License();
// in alternativa è possibile utilizzare uno stream:
license.SetLicense(licensePath);
```

### Vedi anche

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
