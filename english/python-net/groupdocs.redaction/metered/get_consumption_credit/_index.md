---
title: get_consumption_credit method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Gets the consumption credit."
type: docs
url: /python-net/groupdocs.redaction/metered/get_consumption_credit/
is_root: false
weight: 1010
---


## get_consumption_credit

Gets the consumption credit.

```python
def get_consumption_credit(cls):
    ...
```

**Returns:** consumption quantity

### Example

```python
from groupdocs.redaction import Metered

# Assuming metered keys have been set previously
credit = Metered().get_consumption_credit()
print(f"Remaining credit: {credit}")
```

### See Also
* class [`Metered`](/redaction/python-net/groupdocs.redaction/metered/)
