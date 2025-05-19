---
title: redact method
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 20
---

## redact {#groupdocs.redaction.redactions.CustomRedactionContext}

Applies custom redaction to specific document content.
Currently, this is supported only for PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction).
Users can define their own redaction logic, such as AI-based redaction, 
which may be more advanced than simple pattern-based methods.


### Returns 


A [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult) indicating whether the redaction should be applied and the modified content.


```python
def redact(self, context):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| context | [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext) | Contains the document content to be redacted along with related metadata. |



### See Also
* module [`groupdocs.redaction.redactions`](../../)
* class [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult)
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler)
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction)
