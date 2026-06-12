---
title: Metered class
second_title: GroupDocs.Redaction for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.redaction/metered/
is_root: false
weight: 80
---


## Metered class

Manages metered (pay-per-use) licensing.

Metered licenses bill on actual consumption (typically pages or
documents processed). Set the public/private key pair once at
application startup; the wrapper reports usage back to the GroupDocs
license server in the background.

The Metered type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [get_consumption_credit](/redaction/python-net/groupdocs.redaction/metered/get_consumption_credit/) | Return the remaining metered credit for the current key. |
| [get_consumption_quantity](/redaction/python-net/groupdocs.redaction/metered/get_consumption_quantity/) | Return the total metered quantity consumed so far. |
| [set_metered_key](/redaction/python-net/groupdocs.redaction/metered/set_metered_key/#public_key-private_key) | Activate metered billing with the given public/private key pair. |

### See Also
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
