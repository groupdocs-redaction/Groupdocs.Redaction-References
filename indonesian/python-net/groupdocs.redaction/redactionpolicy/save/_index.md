---
title: "metode save"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menyimpan kebijakan redaksi ke file."
type: docs
url: /id/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Menyimpan kebijakan redaksi ke file.

```python
def save(self, file_path):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| file_path | `str` | Jalur ke file. |

### Contoh

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Menyimpan kebijakan redaksi ke aliran.

```python
def save(self, output):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| output | `io.RawIOBase` | Aliran target untuk menyimpan kebijakan. |

**Returns:** None.

### Lihat Juga
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
