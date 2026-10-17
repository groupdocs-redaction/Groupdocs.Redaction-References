---
title: "redact_annotation मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "दस्तावेज़ के भीतर सभी एनोटेशन में मेल खाने वाले पाठ को बदलता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation/
is_root: false
weight: 1030
---


## redact_annotation {#regular_expression-replacement}

दस्तावेज़ के भीतर सभी एनोटेशन में मेल खाने वाले पाठ को बदलता है।

```python
def redact_annotation(self, regular_expression, replacement):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति। |
| replacement | `str` | पाठ्य प्रतिस्थापन। |

**Returns:** Replacement result.

### संबंधित देखें
* class [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/)
