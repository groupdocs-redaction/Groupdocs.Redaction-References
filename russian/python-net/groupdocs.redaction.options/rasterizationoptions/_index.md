---
title: "Класс RasterizationOptions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Предоставляет параметры для конвертации файлов в PDF."
type: docs
url: /ru/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Предоставляет параметры для конвертации файлов в PDF.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

Тип RasterizationOptions раскрывает следующие члены:

### Конструкторы
| Конструктор | Описание |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Инициализирует новый экземпляр. |

### Методы
| Метод | Описание |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Регистрирует расширенную опцию растеризации для применения. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Регистрирует расширенную опцию растеризации для применения. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Свойства
| Свойство | Описание |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | Уровень соответствия PDF. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | Флаг enabled указывает, преобразуются ли все страницы документа в изображения и помещаются в один PDF‑файл. По умолчанию True; установите False, чтобы избежать растеризации. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | Индикатор имеет значение True, если установлены расширенные параметры растеризации. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | Количество страниц, которые будут преобразованы в PDF. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | Индекс первой страницы (нумерация с нуля), которую нужно преобразовать в PDF. |

### Пример

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### См. также
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
