---
title: "SetMeteredKey"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Ενεργοποιεί το προϊόν με κλειδιά Metered."
type: docs
weight: 20
url: /el/net/groupdocs.redaction/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Ενεργοποιεί το προϊόν με κλειδιά Metered.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| publicKey | String | Το δημόσιο κλειδί. |
| privateKey | String | Το ιδιωτικό κλειδί. |

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ενεργοποιήσετε το προϊόν με κλειδιά Metered.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Δείτε επίσης

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
