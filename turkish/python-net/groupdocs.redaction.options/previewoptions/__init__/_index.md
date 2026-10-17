---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Yeni bir PreviewOptions örneği başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

Yeni bir PreviewOptions örneği başlatır. Çıktı akışı kullanım sonrası kapatılacaktır.

```python
def __init__(self, create_page_stream):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Belirli bir sayfa önizlemesi için bir akış oluşturur. |

## __init__ {#create_page_stream-release_page_stream}

Yeni bir PreviewOptions örneği başlatır, çıktı akışının istemciye daha sonraki kullanım için geri döndürülmesine neden olur.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | Belirli bir sayfa önizlemesi için bir akış oluşturur. |
| release_page_stream | `ReleasePageStream` | Sayfa önizlemesi oluşturmanın tamamlandığını bildirir ve çıktı akışını alır. |

### Ayrıca Bakınız
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
