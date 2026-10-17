---
title: "replace_in_column मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "निर्दिष्ट कॉलम और कार्यपत्रक में सभी मेलों को दिए गए प्रतिस्थापन से बदलता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

निर्दिष्ट कॉलम और कार्यपत्रक में सभी मेलों को दिए गए प्रतिस्थापन से बदलता है।

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति। |
| replacement | `str` | पाठ्य प्रतिस्थापन। |
| column | `int` | शून्य-आधारित कॉलम इंडेक्स। |
| sheet | `int` | शून्य-आधारित वर्कशीट इंडेक्स। |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

सभी कार्यपत्रकों में निर्दिष्ट कॉलम में सभी मेलों को दिए गए प्रतिस्थापन से बदलता है।

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति। |
| replacement | `str` | पाठ्य प्रतिस्थापन। |
| column | `int` | शून्य-आधारित कॉलम इंडेक्स। |

**Returns:** Replacement result.

### संबंधित देखें
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
