---
title: "فئة ReplacementOptions"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل خيارات استبدال النص المتطابق."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

يمثل خيارات استبدال النص المتطابق.

اعرف المزيد

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

يعرض نوع ReplacementOptions الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | ينشئ مثيلاً جديدًا من ReplacementOptions بالنص البديل المحدد. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | ينشئ مثيلاً جديدًا من فئة ReplacementOptions مع مستطيل ملون كخيار. |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | إجراء الاستبدال: رسم صندوق أو استبدال النص. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | اللون لخيار `ReplacementType.draw_box` (يُهمل في غير ذلك). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | معالج الحجب المخصص الذي يسمح للمستخدمين بتعريف منطق الحجب الخاص بهم. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | المصفوفة من الفلاتر لتطبيقها مع هذا الحجب. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | قيمة الاستبدال النصي. |

### مثال

```python
from groupdocs.redaction.redactions import ReplacementOptions

# استبدل النص المتطابق بالعنصر النائب "[X]"
repl_opt = ReplacementOptions("[X]")
```

### Guides
أدلة المهام التي تستخدم `ReplacementOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### انظر أيضًا
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
