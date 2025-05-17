---
title: RedactorSettings constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.options/redactorsettings/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance of the RedactorSettings class.



```python
def __init__(self):
    ...
```




## __init__ {#groupdocs.redaction.options.ILogger}

Initializes a new instance of the RedactorSettings class with a given ILogger instance.



```python
def __init__(self, logger):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| logger | [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger) | An instance of a class, implementing ILogger interface |


## __init__ {#groupdocs.redaction.redactions.IRedactionCallback}

Initializes a new instance of the RedactorSettings class with a given IRedactionCallback instance.



```python
def __init__(self, callback):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| callback | groupdocs.redaction.redactions.IRedactionCallback | An instance of a class, implementing IRedactionCallbck interface |


## __init__ {#groupdocs.redaction.integration.ocr.IOcrConnector}

Initializes a new instance of the RedactorSettings class with a given IOcrConnector instance.



```python
def __init__(self, ocr_connector):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| ocr_connector | groupdocs.redaction.integration.ocr.IOcrConnector | A valid implementation of IOcrConnector interface |


## __init__ {#groupdocs.redaction.options.ILogger-groupdocs.redaction.redactions.IRedactionCallback}

Initializes a new instance of the RedactorSettings class with given ILogger and IRedactionCallback instances.



```python
def __init__(self, logger, callback):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| logger | [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger) | An instance of a class, implementing ILogger interface |
| callback | groupdocs.redaction.redactions.IRedactionCallback | An instance of a class, implementing IRedactionCallbck interface |


## __init__ {#groupdocs.redaction.options.ILogger-groupdocs.redaction.redactions.IRedactionCallback-groupdocs.redaction.integration.ocr.IOcrConnector}

Initializes a new instance of the RedactorSettings class with given ILogger, IRedactionCallback and IOcrConnector instances.



```python
def __init__(self, logger, callback, ocr_connector):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| logger | [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger) | An instance of a class, implementing ILogger interface |
| callback | groupdocs.redaction.redactions.IRedactionCallback | An instance of a class, implementing IRedactionCallbck interface |
| ocr_connector | groupdocs.redaction.integration.ocr.IOcrConnector | An instance of IOcrConnector interface implementation. Can be null |



### See Also
* module [`groupdocs.redaction.options`](../../)
* class [`RedactorSettings`](/redaction/python-net/groupdocs.redaction.options/redactorsettings)
