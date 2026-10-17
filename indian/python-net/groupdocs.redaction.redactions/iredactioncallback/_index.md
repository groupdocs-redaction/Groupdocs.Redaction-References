---
title: "IRedactionCallback क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "प्रत्येक रिडैक्शन परिवर्तन पर जानकारी प्राप्त करने के लिए आवश्यक विधियों को परिभाषित करता है और वैकल्पिक रूप से उसे रोकता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

प्रत्येक रिडैक्शन परिवर्तन पर जानकारी प्राप्त करने के लिए आवश्यक विधियों को परिभाषित करता है और वैकल्पिक रूप से उसे रोकता है।

और अधिक जानें:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

IRedactionCallback प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | दस्तावेज़ पर कोई भी रेडैक्शन लागू करने से ठीक पहले ट्रिगर होता है, जिससे लॉगिंग या उसे रोकना संभव होता है। |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
