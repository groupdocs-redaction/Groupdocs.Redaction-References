---
title: apply method
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 20
---

## apply {#groupdocs.redaction.Redaction}

Applies a redaction to the document.


### Returns 


Success or failure and error message in this case


```python
def apply(self, redaction):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| redaction | [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction) | An instance of [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction) to apply |

### Example 


The following example demonstrates applying a single redaction to the document.


## apply {#list}

Applies a set of redactions to the document.


### Returns 


Success or failure and error message in this case


```python
def apply(self, redactions):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| redactions | list | An array of redactions to apply |

### Example 


The following example demonstrates applying a list of redactions to the document.


## apply {#groupdocs.redaction.RedactionPolicy}

Applies a redaction policy to the document.


### Returns 


Success or failure and error message in this case


```python
def apply(self, policy):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| policy | [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy) | Redaction policy |

### Example 


The following example demonstrates how to apply a redaction policy to all files within a given inbound folder, and save to one of outbound folders - for successfully updated files and for failed ones.



### See Also
* module [`groupdocs.redaction`](../../)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor)
