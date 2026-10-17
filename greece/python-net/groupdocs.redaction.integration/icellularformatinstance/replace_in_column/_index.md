---
title: "replace_in_column μέθοδος"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντικαθιστά όλες τις αντιστοιχίες με μια δεδομένη αντικατάσταση στην καθορισμένη στήλη και φύλλο εργασίας."
type: docs
url: /el/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

Αντικαθιστά όλες τις αντιστοιχίες με μια δεδομένη αντικατάσταση στην καθορισμένη στήλη και φύλλο εργασίας.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση για αναζήτηση και αντικατάσταση. |
| replacement | `str` | Κειμενική αντικατάσταση. |
| column | `int` | Δείκτης στήλης με μηδενική βάση. |
| sheet | `int` | Δείκτης φύλλου εργασίας με μηδενική βάση. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

Αντικαθιστά όλες τις αντιστοιχίες με μια δεδομένη αντικατάσταση στην καθορισμένη στήλη σε όλα τα φύλλα εργασίας.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Κανονική έκφραση για αναζήτηση και αντικατάσταση. |
| replacement | `str` | Κειμενική αντικατάσταση. |
| column | `int` | Δείκτης στήλης με μηδενική βάση. |

**Returns:** Replacement result.

### Δείτε επίσης
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
