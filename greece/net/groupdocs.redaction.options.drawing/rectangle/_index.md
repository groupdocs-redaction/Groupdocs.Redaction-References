---
title: "Ορθογώνιο"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Περιγράφει μια ορθογώνια περιοχή σε μια σελίδα ή εικόνα, για παράδειγμα τα όρια κειμένου OCR ή ένα πλαίσιο διαγραφής."
type: docs
weight: 350
url: /el/net/groupdocs.redaction.options.drawing/rectangle/
---
## Rectangle structure

Περιγράφει μια ορθογώνια περιοχή σε μια σελίδα ή εικόνα, για παράδειγμα τα όρια κειμένου OCR ή ένα πλαίσιο επεξεργασίας.

```csharp
public struct Rectangle : IEquatable<Rectangle>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Rectangle](rectangle#constructor)(Point, Size) | Δημιουργεί ένα ορθογώνιο από ένα σημείο επάνω‑αριστερά και το μέγεθος της περιοχής. |
| [Rectangle](rectangle#constructor_1)(int, int, int, int) | Δημιουργεί ένα ορθογώνιο από τις συντεταγμένες των γωνιών και τις διαστάσεις. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/rectangle/empty) { get; } | Ένα ορθογώνιο με μηδενικό πλάτος και ύψος στο αρχικό σημείο. |
| [Height](../../groupdocs.redaction.options.drawing/rectangle/height) { get; set; } | Ύψος της περιοχής, σε εικονοστοιχεία. |
| [IsEmpty](../../groupdocs.redaction.options.drawing/rectangle/isempty) { get; } | Λαμβάνει μια τιμή που υποδεικνύει αν το ορθογώνιο είναι κενό. |
| [Location](../../groupdocs.redaction.options.drawing/rectangle/location) { get; } | Επάνω‑αριστερή γωνία του ορθογωνίου. |
| [Size](../../groupdocs.redaction.options.drawing/rectangle/size) { get; } | Πλάτος και ύψος του ορθογωνίου. |
| [Width](../../groupdocs.redaction.options.drawing/rectangle/width) { get; set; } | Πλάτος της περιοχής, σε εικονοστοιχεία. |
| [X](../../groupdocs.redaction.options.drawing/rectangle/x) { get; set; } | Οριζόντια θέση της πάνω‑αριστερής γωνίας, σε εικονοστοιχεία. |
| [Y](../../groupdocs.redaction.options.drawing/rectangle/y) { get; set; } | Κάθετη θέση της πάνω‑αριστερής γωνίας, σε εικονοστοιχεία. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals_1)(object) | Συγκρίνει αυτό το ορθογώνιο με ένα άλλο αντικείμενο. |
| [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals)(Rectangle) | Συγκρίνει τα όρια με ένα άλλο ορθογώνιο. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/rectangle/gethashcode)() | Επιστρέφει έναν κωδικό κατακερματισμού που προέρχεται από τη θέση και το μέγεθος. |
| override [ToString](../../groupdocs.redaction.options.drawing/rectangle/tostring)() | Επιστρέφει τα όρια σε αναγνώσιμη μορφή. |

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
