---
title: find_format method
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 20
---

## find_format {#str}

Finds format configurations for a given file extension.


### Returns 


If found, instance of [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration), null otherwise


```python
def find_format(self, file_extension):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_extension | str | File extension, format is ".ext" |

### Example 


The following example demonstrates how to get built-in or custom user format handlers.



### See Also
* module [`groupdocs.redaction.configuration`](../../)
* class [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration)
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration)
