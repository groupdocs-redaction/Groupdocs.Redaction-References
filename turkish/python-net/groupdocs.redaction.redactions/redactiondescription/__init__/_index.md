---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Değiştirme bilgisi olmadan RedactionDescription sınıfının yeni bir örneğini başlatır."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

Değiştirme bilgisi olmadan RedactionDescription sınıfının yeni bir örneğini başlatır.

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| redaction_type | `RedactionType` | Kırpılan verinin türü. |
| action_type | `RedactionActionType` | Bu verilere uygulanacak eylem. |
| original_text | `str` | Eşleşen metin, yorum veya açıklama gövdesi. |

## __init__ {#redaction_type-action_type-original_text-replacement}

Değiştirme bilgisiyle RedactionDescription sınıfının yeni bir örneğini başlatır.

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| redaction_type | `RedactionType` | Kırpılan verinin türü. |
| action_type | `RedactionActionType` | Bu verilere uygulanacak eylem. |
| original_text | `str` | Eşleşen metin, yorum veya açıklama gövdesi. |
| replacement | `TextReplacement` | Yerine konulacak metin, eşleşen metin ve orijinal dizedeki konumu. |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

Görüntü alanı değiştirme bilgisiyle yeni bir RedactionDescription başlatır.

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| redaction_type | `RedactionType` | Kırpılan verinin türü. |
| action_type | `RedactionActionType` | Bu verilere uygulanacak eylem. |
| image_area_replacement | `RegionReplacementOptions` | Görüntü alanı değiştirme bilgisi. |
| image_details | `str` | Görüntünün metinsel açıklaması, varsayılan olarak boş bir dizedir. |

### Ayrıca Bakınız
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
