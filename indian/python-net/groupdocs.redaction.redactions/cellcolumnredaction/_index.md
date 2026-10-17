---
title: "CellColumnRedaction क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक टेक्स्ट रेडैक्शन का प्रतिनिधित्व करता है जो स्प्रेडशीट दस्तावेज़ (CSV, Excel आदि) में टेक्स्ट को बदलता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

एक टेक्स्ट रेडैक्शन का प्रतिनिधित्व करता है जो स्प्रेडशीट दस्तावेज़ (CSV, Excel आदि) में टेक्स्ट को बदलता है।

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

CellColumnRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | एक नया CellColumnRedaction आरंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | रेडैक्शन का विवरण, जिसमें उसका नाम और पैरामीटर शामिल हैं। |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | कॉलम और वर्कशीट फ़िल्टर। |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | मेल खाने के लिए नियमित अभिव्यक्ति पैटर्न। |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | पाठ प्रतिस्थापन के प्रकार को निर्दिष्ट करने वाला [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) उदाहरण। ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) से विरासत में मिला) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | ग्राफिक सामग्री से पाठ निकालने के लिए उपयोग किया गया IOcrConnector कार्यान्वयन। ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) से विरासत में मिला) |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.redaction.filters import CellFilter

with Redactor("Sales in September.xlsx") as redactor:
    filter = CellFilter(column_index=1, worksheet_name="Customers")
    regex = r"^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
    redactor.apply(CellColumnRedaction(filter, regex, ReplacementOptions("[customer email]")))
    redactor.save()
```

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
