---
title: "set_license yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Mevcut sürece bir lisans uygulayın."
type: docs
url: /tr/python-net/groupdocs.redaction/license/set_license/
is_root: false
weight: 1010
---


## set_license {#license_source}

Mevcut sürece bir lisans uygulayın.

```python
def set_license(self, license_source):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| license_source |  | Ya bir ``.lic`` dosyasına giden dize yolu ya da lisans baytlarını üreten okunabilir bir dosya benzeri nesne. Dosya benzeri girdiler, köprüye aktarılmadan önce geçici bir dosyaya yazılır. |

| Yükseltir | Açıklama |
| :- | :- |
| `TypeError` | ``license_source`` bir dize yolu ya da okunabilir bir dosya benzeri nesne değilse. |

### Ayrıca Bakınız
* class [`License`](/redaction/python-net/groupdocs.redaction/license/)
