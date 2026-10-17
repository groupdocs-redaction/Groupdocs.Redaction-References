---
title: "طريقة save"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يحفظ سياسة الحجب إلى ملف."
type: docs
url: /ar/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

يحفظ سياسة الحجب إلى ملف.

```python
def save(self, file_path):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| file_path | `str` | المسار إلى الملف. |

### مثال

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

يحفظ سياسة الحجب إلى تدفق.

```python
def save(self, output):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| output | `io.RawIOBase` | دفق الهدف لحفظ السياسة. |

**Returns:** None.

### انظر أيضًا
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
