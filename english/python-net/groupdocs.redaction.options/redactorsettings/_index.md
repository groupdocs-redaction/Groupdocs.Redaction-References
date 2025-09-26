---
title: RedactorSettings class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
weight: 50
url: /python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
---

## RedactorSettings class

Represents redaction settings, allowing to customize the redaction process.



The RedactorSettings type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#) | Initializes a new instance of the RedactorSettings class. |
| [`__init__(self, logger)`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#groupdocs.redaction.options.ilogger) | Initializes a new instance of the RedactorSettings class with a given ILogger instance. |
| [`__init__(self, callback)`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#groupdocs.redaction.redactions.iredactioncallback) | Initializes a new instance of the RedactorSettings class with a given IRedactionCallback instance. |
| [`__init__(self, ocr_connector)`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#groupdocs.redaction.integration.ocr.iocrconnector) | Initializes a new instance of the RedactorSettings class with a given IOcrConnector instance. |
| [`__init__(self, logger, callback)`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#groupdocs.redaction.options.ilogger-groupdocs.redaction.redactions.iredactioncallback) | Initializes a new instance of the RedactorSettings class with given ILogger and IRedactionCallback instances. |
| [`__init__(self, logger, callback, ocr_connector)`](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#groupdocs.redaction.options.ilogger-groupdocs.redaction.redactions.iredactioncallback-groupdocs.redaction.integration.ocr.iocrconnector) | Initializes a new instance of the RedactorSettings class with given ILogger, IRedactionCallback and IOcrConnector instances. |


### Properties
| Property | Description |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger) | Gets or sets an instance of a class, implementing [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger), that is used for logging events and errors. |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback) | Gets or sets an instance of a class, implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector) | Gets or sets an instance of a class, implementing [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector) interface. |



### Remarks 


**Learn more** |
|
 |
 |

### See Also
* module [`groupdocs.redaction.options`](..)
* class [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger)
* class [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector)
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback)
