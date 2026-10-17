---
title: "remove_pages μέθοδος"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αφαιρεί μία ή πολλές σελίδες ανάλογα με τη θέση εκκίνησης, την απόσταση και τον αριθμό."
type: docs
url: /el/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Αφαιρεί μία ή πολλές σελίδες ανάλογα με τη θέση εκκίνησης, την απόσταση και τον αριθμό.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Θέση προέλευσης αναζήτησης, η αρχή ή το τέλος του εγγράφου. |
| index | `int` | Δείκτης αρχικής θέσης (μηδενική βάση). |
| count | `int` | Αριθμός σελίδων προς αφαίρεση. |

**Returns:** Pages removal redaction result.

### Δείτε επίσης
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
