---
title: "save μέθοδος"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αποθηκεύει την πολιτική διαγραφής σε αρχείο."
type: docs
url: /el/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Αποθηκεύει την πολιτική διαγραφής σε αρχείο.

```python
def save(self, file_path):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| file_path | `str` | Διαδρομή προς το αρχείο. |

### Παράδειγμα

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Αποθηκεύει την πολιτική διαγραφής σε ροή.

```python
def save(self, output):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| output | `io.RawIOBase` | Ροή-στόχος για αποθήκευση της πολιτικής. |

**Returns:** None.

### Δείτε επίσης
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
