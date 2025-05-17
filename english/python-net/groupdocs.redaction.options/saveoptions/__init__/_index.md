---
title: SaveOptions constructor
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---

## __init__ {#}

Initializes a new instance with defaults: rasterize to PDF - false, add suffix - false.



```python
def __init__(self):
    ...
```




## __init__ {#bool-str}

Initializes a new instance with given parameters.



```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| rasterize_to_pdf | bool | True, if all pages in the document need to be converted to images and put in a single PDF file |
| suffix | str | This text will be added to the end of file name, if not empty also sets AddSuffix to true |



### See Also
* module [`groupdocs.redaction.options`](../../)
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions)
