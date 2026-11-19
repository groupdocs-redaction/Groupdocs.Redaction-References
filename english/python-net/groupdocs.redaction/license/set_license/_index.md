---
title: set_license method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Sets the GroupDocs.Redaction license from a file path."
type: docs
url: /python-net/groupdocs.redaction/license/set_license/
is_root: false
weight: 1010
---


## set_license {#license_path}

Sets the GroupDocs.Redaction license from a file path.

The method can also accept an open binary stream containing the license data.

```python
def set_license(self, license_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| license_path | `str` | License file path. |

### Example

```python
import os
from groupdocs.redaction import License

def set_license_from_file():
    # Resolve the license path from the environment, with a local fallback
    license_path = os.environ.get("GROUPDOCS_LIC_PATH", "./GroupDocs.Redaction.lic")

    # Apply the license before using any redaction features
    if os.path.exists(license_path):
        License().set_license(license_path)
        print("License set successfully.")
    else:
        print("License file not found. Running in evaluation mode.")
```

## set_license {#license_stream}

Sets the GroupDocs.Redaction license from a stream.

```python
def set_license(self, license_stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| license_stream | `io.RawIOBase` | License stream. |

### Example

```python
import os
from groupdocs.redaction import License

license_path = os.environ.get("GROUPDOCS_LIC_PATH", "./GroupDocs.Redaction.lic")
if os.path.exists(license_path):
    with open(license_path, "rb") as stream:
        License().set_license(stream)
    print("License set successfully.")
else:
    print("License file not found. Running in evaluation mode.")
```

### Aliases

These names call `set_license` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `set_license_file` | `set_license_file(license_path)` |
| `set_license_string` | `set_license_string(license_path)` |
| `set_license_stream` | `set_license_stream(license_stream)` |
| `set_license_streams` | `set_license_streams(license_stream)` |

### See Also
* class [`License`](/redaction/python-net/groupdocs.redaction/license/)
