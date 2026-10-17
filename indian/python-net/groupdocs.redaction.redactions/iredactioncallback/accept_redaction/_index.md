---
title: "accept_redaction मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "दस्तावेज़ पर कोई भी रेडैक्शन लागू करने से ठीक पहले ट्रिगर होता है, जिससे लॉगिंग या उसे रोकना संभव होता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

दस्तावेज़ पर कोई भी रेडैक्शन लागू करने से ठीक पहले ट्रिगर होता है, जिससे लॉगिंग या उसे रोकना संभव होता है।

```python
def accept_redaction(self, description):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| description | `RedactionDescription` | विशिष्ट मैच प्रकार, मानदंड, पाठ और स्थिति के बारे में जानकारी शामिल है। |

**Returns:** bool: True to accept the redaction, False to decline it.

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
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
