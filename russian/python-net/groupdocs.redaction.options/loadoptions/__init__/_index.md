---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр класса LoadOptions."
type: docs
url: /ru/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

Инициализирует новый экземпляр класса LoadOptions.

```python
def __init__(self):
    ...
```

## __init__ {#password}

Инициализирует новый экземпляр LoadOptions с указанным паролем.

```python
def __init__(self, password):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| password | `str` | Пароль для защищённых файлов. |

### Пример

```python
    from groupdocs.redaction.options import LoadOptions

    # Загрузить документ, защищённый паролем
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

Инициализирует новый экземпляр LoadOptions с указанным флагом предварительной растеризации.

```python
def __init__(self, pre_rasterize):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| pre_rasterize | `bool` | Если True, принудительно выполнять растеризацию при загрузке. |

## __init__ {#password-pre_rasterize}

Инициализирует новый экземпляр LoadOptions с указанным паролем.

Если `pre_rasterize` равно True, растеризация принудительно выполняется при загрузке документа.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| password | `str` | Пароль для защищённых файлов. |
| pre_rasterize | `bool` | Если True, принудительно выполнять растеризацию при загрузке. |

### Пример

```python
from groupdocs.redaction.options import LoadOptions

# Загрузить документ, защищённый паролем
load_opt = LoadOptions("mypassword")
```

### См. также
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
