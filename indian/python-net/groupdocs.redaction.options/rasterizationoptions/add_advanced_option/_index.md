---
title: "add_advanced_option मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत करता है।

```python
def add_advanced_option(self, option_type):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | चयनित इफ़ेक्ट प्रकार (ग्रेस्केल, बॉर्डर, आदि) के बारे में जानकारी प्रदान करता है। |

### उदाहरण

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत करता है।

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | चयनित इफ़ेक्ट प्रकार (ग्रेस्केल, बॉर्डर, आदि) के बारे में जानकारी प्रदान करता है। |
| parameters | `dict[str, str]` | दिए गए इफ़ेक्ट के पैरामीटर, जैसे घूर्णन कोण। |

### उदाहरण

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# निर्मित‑इन इफ़ेक्ट लागू करें
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# कस्टम सेटिंग्स के साथ इफ़ेक्ट लागू करें, उदाहरण के लिए, 10 इकाइयों का बॉर्डर
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### संबंधित देखें
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
