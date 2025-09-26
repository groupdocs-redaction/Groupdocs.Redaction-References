---
title: RedactionPolicy class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
weight: 80
url: /python-net/groupdocs.redaction/redactionpolicy/
is_root: false
---

## RedactionPolicy class

Represents a sanitization policy, containing a set of specific redactions to apply.



The RedactionPolicy type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#) | Creates a new instance of Redaction policy. |
| [`__init__(self, redactions)`](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#list) | Creates a new instance of Redaction policy with a specific list of redactions. |


### Properties
| Property | Description |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions) | Gets an array of fully configured [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)-derived classes. |


### Methods
| Method | Description |
| :- | :- |
| [`load(, file_path)`](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#str) | Loads an instance of [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy) from a file path. |
| [`load(, input)`](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#io.rawiobase) | Loads an instance of [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy) from a stream. |
| [`save(self, file_path)`](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#str) | Saves the redaction policy to a file. |
| [`save(self, output)`](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#io.rawiobase) | Saves the redaction policy to a stream. |



### Remarks 


**Learn more** |
|
 |
 |

### Example 


The following example demonstrates how to apply a redaction policy to all files within a given inbound folder, and save to one of outbound folders - for successfully updated files and for failed ones.


The following example contains a sample XML policy file with sample configurations for all types of redactions.

### See Also
* module [`groupdocs.redaction`](..)
* class [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction)
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy)
