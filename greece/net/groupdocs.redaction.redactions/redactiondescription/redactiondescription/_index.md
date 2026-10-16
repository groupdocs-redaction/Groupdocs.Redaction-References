---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription χωρίς πληροφορίες αντικατάστασης."
type: docs
weight: 10
url: /el/net/groupdocs.redaction.redactions/redactiondescription/redactiondescription/
---
## RedactionDescription(RedactionType, RedactionActionType, string) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription χωρίς πληροφορίες αντικατάστασης.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| redactionType | RedactionType | Τύπος των δεδομένων που διαγράφονται |
| actionType | RedactionActionType | Ενέργεια που θα εκτελεστεί σε αυτά τα δεδομένα |
| originalText | String | Ταιριασμένο κείμενο, σχόλιο ή σώμα σημείωσης |

### Δείτε επίσης

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, string, TextReplacement) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription με πληροφορίες αντικατάστασης.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText, TextReplacement replacement)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| redactionType | RedactionType | Τύπος των δεδομένων που διαγράφονται |
| actionType | RedactionActionType | Ενέργεια που θα εκτελεστεί σε αυτά τα δεδομένα |
| originalText | String | Ταιριασμένο κείμενο, σχόλιο ή σώμα σημείωσης |
| αντικατάσταση | TextReplacement | Κείμενο αντικατάστασης, ταιριασμένο κείμενο και η θέση του μέσα στην αρχική συμβολοσειρά |

### Δείτε επίσης

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [TextReplacement](../../textreplacement)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, RegionReplacementOptions, string) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης RedactionDescription με πληροφορίες αντικατάστασης περιοχής εικόνας.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    RegionReplacementOptions imageAreaReplacement, string imageDetails)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| redactionType | RedactionType | Τύπος των δεδομένων που διαγράφονται |
| actionType | RedactionActionType | Ενέργεια που θα εκτελεστεί σε αυτά τα δεδομένα |
| imageAreaReplacement | RegionReplacementOptions | Πληροφορίες αντικατάστασης περιοχής εικόνας |
| imageDetails | String | Κειμενική περιγραφή εικόνας, εξ ορισμού είναι String.Empty |

### Δείτε επίσης

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RegionReplacementOptions](../../regionreplacementoptions)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
