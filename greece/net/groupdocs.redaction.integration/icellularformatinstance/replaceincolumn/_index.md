---
title: "ReplaceInColumn"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντικαθιστά όλες τις αντιστοιχίες με μια δεδομένη αντικατάσταση στην καθορισμένη στήλη και φύλλο εργασίας."
type: docs
weight: 20
url: /el/net/groupdocs.redaction.integration/icellularformatinstance/replaceincolumn/
---
## ReplaceInColumn(Regex, string, int, int) {#replaceincolumn_1}

Αντικαθιστά όλες τις αντιστοιχίες με μια δεδομένη αντικατάσταση στην καθορισμένη στήλη και φύλλο εργασίας.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column, 
    int sheet)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| regularExpression | Regex | Κανονική έκφραση για αναζήτηση και αντικατάσταση |
| αντικατάσταση | String | Κειμενική αντικατάσταση |
| στήλη | Int32 | Δείκτης στήλης μηδενικής βάσης |
| φύλλο | Int32 | Δείκτης φύλλου εργασίας με βάση το μηδέν |

### Τιμή Επιστροφής

Αποτέλεσμα αντικατάστασης

### Δείτε επίσης

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

---

## ReplaceInColumn(Regex, string, int) {#replaceincolumn}

Αντικαθιστά όλες τις αντιστοιχίες με μια δεδομένη αντικατάσταση στην καθορισμένη στήλη σε όλα τα φύλλα εργασίας.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| regularExpression | Regex | Κανονική έκφραση για αναζήτηση και αντικατάσταση |
| αντικατάσταση | String | Κειμενική αντικατάσταση |
| στήλη | Int32 | Δείκτης στήλης μηδενικής βάσης |

### Τιμή Επιστροφής

Αποτέλεσμα αντικατάστασης

### Δείτε επίσης

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
