---
title: "метод add_advanced_option"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Регистрирует расширенную опцию растеризации для применения."
type: docs
url: /ru/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Регистрирует расширенную опцию растеризации для применения.

```python
def add_advanced_option(self, option_type):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Предоставляет информацию о выбранном типе эффекта (оттенки серого, граница и т.д.). |

### Пример

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Регистрирует расширенную опцию растеризации для применения.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Предоставляет информацию о выбранном типе эффекта (оттенки серого, граница и т.д.). |
| parameters | `dict[str, str]` | Параметры данного эффекта, такие как угол вращения. |

### Пример

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Применить встроенные эффекты
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Применить эффект с пользовательскими настройками, например, границу в 10 единиц
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### См. также
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
