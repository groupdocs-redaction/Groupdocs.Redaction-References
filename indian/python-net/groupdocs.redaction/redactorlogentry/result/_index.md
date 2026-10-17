---
title: "result प्रॉपर्टी"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "DocumentFormatInstance द्वारा लौटाया गया परिणाम।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

[`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) द्वारा लौटाया गया परिणाम।

सभी मेटाडेटा redaction प्रत्येक मेटाडेटा आइटम पर अलग‑अलग लागू होते हैं, और यदि किसी मेटाडेटा आइटम का redaction विफल हो भी जाता है, तो बाकी मेटाडेटा आइटम अपडेट हो जाएंगे। आप `ErrorMessage` प्रॉपर्टी में विफल, छोड़े गए (अस्वीकृत) मेटाडेटा आइटमों और उनके कारणों की सूची पा सकते हैं, जो [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/) में है।

### Definition:
```python
@property
def result(self):
    ...
```

### संबंधित देखें
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
