---
title: get_consumption_quantity method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Retrieves the amount of megabytes processed."
type: docs
url: /python-net/groupdocs.redaction/metered/get_consumption_quantity/
is_root: false
weight: 1020
---


## get_consumption_quantity

Retrieves the amount of megabytes processed.

```python
def get_consumption_quantity(cls):
    ...
```

**Returns:** consumption quantity

### Example

```python
from groupdocs.redaction import Metered

# Replace with your actual metered keys
public_key = "your_public_key"
private_key = "your_private_key"

# Apply the metered license
Metered().set_metered_key(public_key, private_key)

# Query the processed megabytes
mb_processed = Metered().get_consumption_quantity()
print(f"Processed megabytes: {mb_processed}")
```

### See Also
* class [`Metered`](/redaction/python-net/groupdocs.redaction/metered/)
