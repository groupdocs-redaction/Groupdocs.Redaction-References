---
title: "Metered"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Παρέχει μεθόδους που επιτρέπουν την ενεργοποίηση του προϊόντος με άδεια Metered και την ανάκτηση του ποσού των επεξεργασμένων MB. Μάθετε περισσότερα για τις άδειες Metered εδώhttps//purchase.groupdocs.com/faqs/licensing/metered."
type: docs
weight: 280
url: /el/net/groupdocs.redaction/metered/
---
## Metered class

Παρέχει μεθόδους που επιτρέπουν την ενεργοποίηση του προϊόντος με άδεια Metered και την ανάκτηση του ποσού των επεξεργασμένων MB. Μάθετε περισσότερα για τις άδειες Metered [εδώ](https://purchase.groupdocs.com/faqs/licensing/metered).

```csharp
public class Metered
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Metered](metered)() | Αρχικοποιεί ένα νέο αντίτυπο της κλάσης Metered. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | Ενεργοποιεί το προϊόν με κλειδιά Metered. |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | Λαμβάνει το πιστωτικό κατανάλωσης. |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | Ανακτά το ποσό των επεξεργασμένων MB. |

### Παρατηρήσεις

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ενεργοποιήσετε το προϊόν με κλειδιά Metered.

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

το αρχείο jar του component:

```csharp
Metered matered = new Metered();
matered.setMeteredKey("PublicKey", "PrivateKey");
```

### Δείτε επίσης

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
