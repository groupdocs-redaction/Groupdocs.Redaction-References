---
title: "result özelliği"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "DocumentFormatInstance tarafından döndürülen sonuç."
type: docs
url: /tr/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

[`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) tarafından döndürülen sonuç.

Tüm metadata redaksiyonları her metadata öğesine ayrı ayrı uygulanır ve bir metadata öğesi redaksiyonu başarısız olsa bile, diğer metadata öğeleri güncellenir. Başarısız, atlanan (reddedilen) metadata öğeleri ve bunların nedenleri listesini `ErrorMessage` özelliğinde, [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/) içinde bulabilirsiniz.

### Definition:
```python
@property
def result(self):
    ...
```

### Ayrıca Bakınız
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
