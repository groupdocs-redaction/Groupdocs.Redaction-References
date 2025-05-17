---
title: save method
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 50
---

## save {#}

Saves the document to a file with the following options: AddSuffix = true, RasterizeToPDF = true.


### Returns 


Path to redacted document


```python
def save(self):
    ...
```




## save {#groupdocs.redaction.options.SaveOptions}

Saves the document to a file.


### Returns 


Path to redacted document


```python
def save(self, save_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| save_options | groupdocs.redaction.options.SaveOptions | Options to add suffix or rasterize |

### Example 


The following example demonstrates how to save a document using SaveOptions.


## save {#io.RawIOBase-groupdocs.redaction.options.RasterizationOptions}

Saves the document to a stream, including custom location.



```python
def save(self, document, rasterization_options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| document | io.RawIOBase | Target stream |
| rasterization_options | groupdocs.redaction.options.RasterizationOptions | Options to rasterize or not and to specify pages for rasterization |

### Example 


The following example demonstrates how to set options for the rasterization process.



### See Also
* module [`groupdocs.redaction`](../../)
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor)
