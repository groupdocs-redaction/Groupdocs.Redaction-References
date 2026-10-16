---
title: "GetConsumptionQuantity"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Ανακτά το ποσό των επεξεργασμένων MB."
type: docs
weight: 40
url: /el/net/groupdocs.redaction/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Ανακτά το ποσό των επεξεργασμένων MB.

```csharp
public static decimal GetConsumptionQuantity()
```

### Τιμή Επιστροφής

ποσότητα κατανάλωσης

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ανακτήσετε το ποσό των επεξεργασμένων MB.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### Δείτε επίσης

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
