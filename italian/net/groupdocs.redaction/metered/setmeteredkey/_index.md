---
title: "SetMeteredKey"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Attiva il prodotto con chiavi a consumo."
type: docs
weight: 20
url: /it/net/groupdocs.redaction/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Attiva il prodotto con chiavi a consumo.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| publicKey | String | La chiave pubblica. |
| privateKey | String | La chiave privata. |

### Esempi

Il seguente esempio dimostra come attivare il prodotto con chiavi a consumo.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Vedi anche

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
