---
title: "FromName"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Crea un colore dal nome specificato di un colore noto. Se il nome non è un nome di colore noto viene generata un'eccezione."
type: docs
weight: 1440
url: /it/net/groupdocs.redaction.options.drawing/color/fromname/
---
## Color.FromName method

Crea un colore dal nome specificato di un colore noto. Se *name* non è un nome di colore noto, viene sollevata un'eccezione.

```csharp
public static Color FromName(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome di un colore noto, come `Red` o `Black`. |

### Valore di ritorno

Il colore denominato.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *name* è `null`. |
| ArgumentException | *name* non è un nome di colore noto. |

### Vedi anche

* struct [Color](../../color)
* namespace [GroupDocs.Redaction.Options.Drawing](../../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
