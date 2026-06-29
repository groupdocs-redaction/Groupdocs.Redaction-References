---
title: result property
second_title: GroupDocs.Redaction for Python via .NET API References
description: "The result returned by DocumentFormatInstance."
type: docs
url: /python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

The result returned by [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/).

All metadata redactions apply to each metadata item separately, and even if a metadata item redaction fails, the rest of the metadata items will be updated. You can find a list of failed, skipped (rejected) metadata items and reasons for that in the `ErrorMessage` property of [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

### Definition:
```python
@property
def result(self):
    ...
```

### See Also
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
