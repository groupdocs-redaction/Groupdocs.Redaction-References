---
title: DocumentFormatInstance class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
weight: 10
url: /groupdocs.redaction.integration/documentformatinstance/
is_root: false
---

## DocumentFormatInstance class

Represents a specific format of a document. Implement this class to add your own document types.



The DocumentFormatInstance type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password) | Gets or sets a password for password protected documents. |


### Methods
| Method | Description |
| :- | :- |
| [`initialize(self, config, settings)`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#groupdocs.redaction.configuration.documentformatconfiguration-groupdocs.redaction.options.redactorsettings) | Performs initialization of the instance of document format handler. |
| [`load(self, input)`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#io.rawiobase) | Loads the document from a stream. |
| [`save(self, output)`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#io.rawiobase) | Saves the document to a stream. |
| [`is_redaction_accepted(self, description)`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#groupdocs.redaction.redactions.redactiondescription) | Checks for [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback) implementation and invokes it, if specified. |
| [`perform_binary_check(self, input)`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#io.rawiobase) | Checks if the given stream contains a document, supported by this format instance. |



### Remarks 


**Learn more** |
|
 |

### Example 


The following example demonstrates how to create an empty stub for a custom format handler.

The following example demonstrates how to use the initialization data.

### See Also
* module [`groupdocs.redaction.integration`](..)
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback)
