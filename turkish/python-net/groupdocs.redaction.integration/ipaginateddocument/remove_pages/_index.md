---
title: "remove_pages yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Başlangıç konumu, offset ve sayıya göre bir veya birden fazla sayfayı kaldırır."
type: docs
url: /tr/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

Başlangıç konumu, offset ve sayıya göre bir veya birden fazla sayfayı kaldırır.

```python
def remove_pages(self, origin, index, count):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| origin | `PageSeekOrigin` | Arama başlangıç konumu, belgenin başı ya da sonu. |
| index | `int` | Başlangıç konumu indeksi (0 tabanlı). |
| count | `int` | Kaldırılacak sayfa sayısı. |

**Returns:** Pages removal redaction result.

### Ayrıca Bakınız
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
