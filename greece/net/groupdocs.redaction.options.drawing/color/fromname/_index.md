---
title: "ΑπόΌνομα"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Δημιουργεί ένα χρώμα από το καθορισμένο όνομα ενός γνωστού χρώματος. Εάν το όνομα δεν είναι γνωστό όνομα χρώματος, ρίχνεται εξαίρεση."
type: docs
weight: 1440
url: /el/net/groupdocs.redaction.options.drawing/color/fromname/
---
## Color.FromName method

Δημιουργεί ένα χρώμα από το καθορισμένο όνομα ενός γνωστού χρώματος. Εάν το *name* δεν είναι γνωστό όνομα χρώματος, ρίχνεται μια εξαίρεση.

```csharp
public static Color FromName(string name)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | String | Το όνομα ενός γνωστού χρώματος, όπως `Red` ή `Black`. |

### Τιμή Επιστροφής

Το ονομασμένο χρώμα.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *name* είναι `null`. |
| ArgumentException | *name* δεν είναι γνωστό όνομα χρώματος. |

### Δείτε επίσης

* struct [Color](../../color)
* namespace [GroupDocs.Redaction.Options.Drawing](../../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
