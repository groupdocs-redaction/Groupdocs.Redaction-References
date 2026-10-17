---
title: "خاصية result"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "النتيجة التي تم إرجاعها بواسطة DocumentFormatInstance."
type: docs
url: /ar/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

النتيجة التي تُرجعها [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/).

تنطبق جميع عمليات redaction للبيانات الوصفية على كل عنصر من عناصر البيانات الوصفية بشكل منفصل، وحتى إذا فشل redaction لعنصر بيانات وصفية، سيتم تحديث باقي عناصر البيانات الوصفية. يمكنك العثور على قائمة بالعناصر الفاشلة، المتخطاة (المرفوضة) وأسباب ذلك في خاصية `ErrorMessage` لـ [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

### Definition:
```python
@property
def result(self):
    ...
```

### انظر أيضًا
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
