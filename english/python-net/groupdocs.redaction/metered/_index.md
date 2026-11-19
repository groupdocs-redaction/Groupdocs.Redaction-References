---
title: Metered class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Provides methods which allow to activate the product with a Metered license and retrieve the amount of MBs processed."
type: docs
url: /python-net/groupdocs.redaction/metered/
is_root: false
weight: 60
---


## Metered class

Provides methods which allow to activate the product with a Metered license and retrieve the amount of MBs processed.

Learn more:
- More about licensing: https://purchase.groupdocs.com/faqs/licensing

The Metered type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/metered/__init__/) | Initializes a new instance of the Metered class. |

### Methods
| Method | Description |
| :- | :- |
| [get_consumption_credit](/redaction/python-net/groupdocs.redaction/metered/get_consumption_credit/) | Gets the consumption credit. |
| [get_consumption_quantity](/redaction/python-net/groupdocs.redaction/metered/get_consumption_quantity/) | Retrieves the amount of megabytes processed. |
| [set_metered_key](/redaction/python-net/groupdocs.redaction/metered/set_metered_key/#public_key-private_key) | Activates the product with Metered keys. |

### Example

```python
from groupdocs.redaction import Metered

def set_metered_license():
    public_key = "*****"
    private_key = "*****"

    if "*" in public_key or "*" in private_key:
        print("Provide real metered keys to enable metered licensing.")
        return

    Metered().set_metered_key(public_key, private_key)

    quantity = Metered().get_consumption_quantity()
    credit = Metered().get_consumption_credit()
    print(f"Consumption quantity: {quantity}, credit: {credit}")
```

### See Also
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
