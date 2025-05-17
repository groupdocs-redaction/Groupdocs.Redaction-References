---
title: load method
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 20
---

## load {#str}

Loads an instance of [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy) from a file path.


### Returns 


Redaction policy


```python
def load(self, file_path):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_path | str | Path to XML file |

### Example 


The following example demonstrates how to apply a redaction policy to all files within a given inbound folder, and save to one of outbound folders - for successfully updated files and for failed ones.


The following example contains a sample XML policy file with sample configurations for all types of redactions.


## load {#io.RawIOBase}

Loads an instance of [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy) from a stream.


### Returns 


Redaction policy


```python
def load(self, input):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| input | io.RawIOBase | Stream containing XML configuration |

### Example 


The following example demonstrates how to apply a redaction policy to all files within a given inbound folder, and save to one of outbound folders - for successfully updated files and for failed ones.


The following example contains a sample XML policy file with sample configurations for all types of redactions.



### See Also
* module [`groupdocs.redaction`](../../)
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy)
