---
title: ICustomRedactionHandler class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
weight: 90
url: /python-net/groupdocs.redaction.redactions/icustomredactionhandler/
is_root: false
---

## ICustomRedactionHandler class

Provides an interface for implementing custom redaction logic.



The ICustomRedactionHandler type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [`redact(self, context)`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/#groupdocs.redaction.redactions.customredactioncontext) | Applies custom redaction to specific document content.<br/>Currently, this is supported only for PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction).<br/>Users can define their own redaction logic, such as AI-based redaction, <br/>which may be more advanced than simple pattern-based methods. |



### See Also
* module [`groupdocs.redaction.redactions`](..)
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction)
