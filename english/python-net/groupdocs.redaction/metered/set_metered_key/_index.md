---
title: set_metered_key method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Activates the product with Metered keys."
type: docs
url: /python-net/groupdocs.redaction/metered/set_metered_key/
is_root: false
weight: 1030
---


## set_metered_key {#public_key-private_key}

Activates the product with Metered keys.

```python
def set_metered_key(self, public_key, private_key):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| public_key | `str` | The public key. |
| private_key | `str` | The private key. |

### Example

```python
from groupdocs.redaction import Metered

public_key = "*****"
private_key = "*****"

# Skip the call until real keys are supplied (placeholder keys are rejected)
if "*" in public_key or "*" in private_key:
    print("Provide real metered keys to enable metered licensing.")
else:
    Metered().set_metered_key(public_key, private_key)

    # Query the current metered consumption
    quantity = Metered().get_consumption_quantity()
    credit = Metered().get_consumption_credit()
    print(f"Consumption quantity: {quantity}, credit: {credit}")
```

### Aliases

These names call `set_metered_key` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `set_metered_key_file` | `set_metered_key_file(public_key, private_key)` |
| `set_metered_key_string` | `set_metered_key_string(public_key, private_key)` |

### See Also
* class [`Metered`](/redaction/python-net/groupdocs.redaction/metered/)
