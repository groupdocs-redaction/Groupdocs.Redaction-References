---
title: from_argb method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Builds a color from a packed 32-bit value in ARGB order."
type: docs
url: /python-net/groupdocs.redaction.options.drawing/color/from_argb/
is_root: false
weight: 1020
---


## from_argb {#argb}

Builds a color from a packed 32-bit value in ARGB order.

```python
def from_argb(cls, argb):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| argb | `int` | Packed alpha, red, green, and blue values. |

**Returns:** Color: A color that can be assigned to redaction options.

## from_argb {#alpha-red-green-blue}

Builds a color from separate channel values.

```python
def from_argb(cls, alpha, red, green, blue):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| alpha | `int` | Opacity from 0 to 255. |
| red | `int` | Red channel from 0 to 255. |
| green | `int` | Green channel from 0 to 255. |
| blue | `int` | Blue channel from 0 to 255. |

**Returns:** Color: A color that can be assigned to redaction options.

### Example

```python
from groupdocs.redaction.options.drawing import Color

# Create a semi‑transparent red color
color = Color.from_argb(128, 255, 0, 0)
```

### Aliases

These names call `from_argb` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `from_argb_int32` | `from_argb_int32(alpha, red, green, blue)`<br>`from_argb_int32(argb)` |

### See Also
* class [`Color`](/redaction/python-net/groupdocs.redaction.options.drawing/color/)
