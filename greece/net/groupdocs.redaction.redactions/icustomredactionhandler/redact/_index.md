---
title: "Απόκρυψη"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Εφαρμόζει προσαρμοσμένη απόκρυψη σε συγκεκριμένο περιεχόμενο εγγράφου. Προς το παρόν, αυτό υποστηρίζεται μόνο για PDF PageAreaRedactiongroupdocs.redaction.redactions/pagearearedaction. Οι χρήστες μπορούν να ορίσουν τη δική τους λογική απόκρυψης, όπως η AIbased απόκρυψη, η οποία μπορεί να είναι πιο προχωρημένη από τις απλές μεθόδους patternbased."
type: docs
weight: 10
url: /el/net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
---
## ICustomRedactionHandler.Redact method

Εφαρμόζει προσαρμοσμένη απόκρυψη σε συγκεκριμένο περιεχόμενο εγγράφου. Προς το παρόν, αυτό υποστηρίζεται μόνο για PDF [`PageAreaRedaction`](../../pagearearedaction). Οι χρήστες μπορούν να ορίσουν τη δική τους λογική απόκρυψης, όπως η AI-based απόκρυψη, η οποία μπορεί να είναι πιο προχωρημένη από τις απλές μεθόδους pattern-based.

```csharp
public CustomRedactionResult Redact(CustomRedactionContext context)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πλαίσιο | CustomRedactionContext | Περιέχει το περιεχόμενο του εγγράφου που θα υποβληθεί σε απόκρυψη μαζί με τα σχετικά μεταδεδομένα. |

### Τιμή Επιστροφής

Ένα [`CustomRedactionResult`](../../customredactionresult) που υποδεικνύει εάν η απόκρυψη πρέπει να εφαρμοστεί και το τροποποιημένο περιεχόμενο.

### Δείτε επίσης

* class [CustomRedactionResult](../../customredactionresult)
* class [CustomRedactionContext](../../customredactioncontext)
* interface [ICustomRedactionHandler](../../icustomredactionhandler)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
