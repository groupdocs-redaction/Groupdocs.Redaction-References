---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक नया PreviewOptions इंस्टेंस प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

एक नया PreviewOptions इंस्टेंस प्रारंभ करता है। आउटपुट स्ट्रीम उपयोग के बाद बंद कर दी जाएगी।

```python
def __init__(self, create_page_stream):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | एक विशिष्ट पेज प्रीव्यू के लिए स्ट्रीम बनाता है। |

## __init__ {#create_page_stream-release_page_stream}

एक नया PreviewOptions इंस्टेंस प्रारंभ करता है, जिससे आउटपुट स्ट्रीम क्लाइंट को आगे उपयोग के लिए वापस कर दी जाती है।

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | एक विशिष्ट पेज प्रीव्यू के लिए स्ट्रीम बनाता है। |
| release_page_stream | `ReleasePageStream` | संदेश देता है कि पेज प्रीव्यू जनरेशन समाप्त हो गया है और आउटपुट स्ट्रीम प्राप्त करता है। |

### संबंधित देखें
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
