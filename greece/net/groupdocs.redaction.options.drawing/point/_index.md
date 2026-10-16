---
title: "Σημείο"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αναγνωρίζει μια μετατόπιση pixel σε μια σελίδα ή εικόνα, συνήθως στην επάνω αριστερή γωνία μιας περιοχής διαγραφής."
type: docs
weight: 340
url: /el/net/groupdocs.redaction.options.drawing/point/
---
## Point structure

Καθορίζει μια μετατόπιση εικονοστοιχείου σε μια σελίδα ή εικόνα, συνήθως την επάνω αριστερή γωνία μιας περιοχής επεξεργασίας.

```csharp
public struct Point : IEquatable<Point>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Point](point)(int, int) | Δημιουργεί ένα σημείο για την αρχή μιας περιοχής διαγραφής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/point/empty) { get; } | Ένα σημείο στην αρχή (0, 0). |
| [X](../../groupdocs.redaction.options.drawing/point/x) { get; } | Οριζόντια μετατόπιση από την αριστερή άκρη, σε pixel. |
| [Y](../../groupdocs.redaction.options.drawing/point/y) { get; } | Κατακόρυφη μετατόπιση από την επάνω άκρη, σε pixel. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals_1)(object) | Συγκρίνει αυτό το σημείο με ένα άλλο αντικείμενο. |
| [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals)(Point) | Συγκρίνει τις συντεταγμένες με ένα άλλο σημείο. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/point/gethashcode)() | Επιστρέφει έναν κωδικό κατακερματισμού που προέρχεται από τις συντεταγμένες. |
| override [ToString](../../groupdocs.redaction.options.drawing/point/tostring)() | Επιστρέφει τις συντεταγμένες σε αναγνώσιμη μορφή. |

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
