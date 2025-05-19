---
title: accept_redaction method
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 20
---

## accept_redaction {#groupdocs.redaction.redactions.RedactionDescription}

This call is triggered right before applying any redaction to the document and allows to log or forbid it.


### Returns 


Return true to accept or false to decline particular match redaction


```python
def accept_redaction(self, description):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| description | [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription) | Contains information about particular match type, criteria, text and position |



### See Also
* module [`groupdocs.redaction.redactions`](../../)
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback)
