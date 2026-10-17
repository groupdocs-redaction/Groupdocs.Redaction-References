---
title: "save मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "रेडैक्शन नीति को फ़ाइल में सहेजता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

रेडैक्शन नीति को फ़ाइल में सहेजता है।

```python
def save(self, file_path):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| file_path | `str` | फ़ाइल का पथ। |

### उदाहरण

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

रेडैक्शन नीति को स्ट्रीम में सहेजता है।

```python
def save(self, output):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| output | `io.RawIOBase` | नीति को सहेजने के लिए लक्ष्य स्ट्रीम। |

**Returns:** None.

### संबंधित देखें
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
