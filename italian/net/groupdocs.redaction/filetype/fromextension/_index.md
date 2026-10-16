---
title: "FromExtension"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Mappa l'estensione del file al tipo di file."
type: docs
weight: 500
url: /it/net/groupdocs.redaction/filetype/fromextension/
---
## FileType.FromExtension method

Mappa l'estensione del file al tipo di file.

```csharp
public static FileType FromExtension(string extension)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| estensione | String | Estensione del file (incluso il punto "."). |

### Valore di ritorno

Quando il tipo di file è supportato lo restituisce, altrimenti restituisce il tipo di file predefinito [`Unknown`](../unknown).

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Generato quando *extension* è null o una stringa vuota. |

### Vedi anche

* class [FileType](../../filetype)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
