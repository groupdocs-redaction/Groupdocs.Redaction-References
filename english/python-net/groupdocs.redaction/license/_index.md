---
title: License class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Provides methods for applying a license."
type: docs
url: /python-net/groupdocs.redaction/license/
is_root: false
weight: 50
---


## License class

Provides methods for applying a license.

- More about licensing: https://purchase.groupdocs.com/faqs/licensing

The License type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/license/__init__/) | Initializes a License instance. |

### Methods
| Method | Description |
| :- | :- |
| [set_license](/redaction/python-net/groupdocs.redaction/license/set_license/#license_path) | Sets the GroupDocs.Redaction license from a file path. |
| [set_license](/redaction/python-net/groupdocs.redaction/license/set_license/#license_stream) | Sets the GroupDocs.Redaction license from a stream. |

### Properties
| Property | Description |
| :- | :- |
| [is_licensed](/redaction/python-net/groupdocs.redaction/license/is_licensed/) | The property returns True if a valid license has been applied; otherwise, returns False when the component is running in evaluation mode. |

### Example

```python
import os
from groupdocs.redaction import License

def set_license():
    # Resolve the license path from the environment, with a local fallback
    license_path = os.environ.get("GROUPDOCS_LIC_PATH", "./GroupDocs.Redaction.lic")
    if os.path.exists(license_path):
        License().set_license(license_path)
        print("License set successfully.")
    else:
        print("License file not found. Running in evaluation mode.")
```

### See Also
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
