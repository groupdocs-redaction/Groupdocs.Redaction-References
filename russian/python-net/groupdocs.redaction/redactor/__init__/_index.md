---
title: "__init__ конструктор"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Инициализирует новый экземпляр Redactor, используя путь к файлу."
type: docs
url: /ru/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

Инициализирует новый экземпляр Redactor, используя путь к файлу.

```python
def __init__(self, file_path):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| file_path | `str` | Путь к файлу. |

### Пример

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # Выполните операции редактирования здесь
    pass
```

## __init__ {#document}

Инициализирует новый экземпляр [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) с использованием потока.

```python
def __init__(self, document):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| document | `io.RawIOBase` | Исходный поток документа. |

### Пример

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # Откройте документ как бинарный поток
    with open("./sample.pdf", "rb") as stream:
        # Загрузите документ из потока
        with Redactor(stream) as redactor:
            # Выполните редактирование здесь
            pass
```

## __init__ {#file_path-load_options}

Инициализирует новый экземпляр [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) для защищённого паролем документа, используя его путь.

```python
def __init__(self, file_path, load_options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| file_path | `str` | Путь к файлу. |
| load_options | `LoadOptions` | Параметры, включая пароль. |

### Пример

```python
from groupdocs.redaction import Redactor

# Загрузите защищённый паролем документ из пути к файлу
with Redactor("protected.docx") as redactor:
    # Выполните операции редактирования здесь
    pass
```

## __init__ {#file_path-load_options-settings}

Инициализирует новый экземпляр Redactor для защищённого паролем документа, используя его путь и настройки.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| file_path | `str` | Путь к файлу. |
| load_options | `LoadOptions` | Опции, зависящие от файла, включая пароль. |
| settings | `RedactorSettings` | Настройки по умолчанию для процесса редактирования. |

### Пример

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

Инициализирует новый экземпляр Redactor для защищённого паролем документа, используя поток.

```python
def __init__(self, document, load_options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| document | `io.RawIOBase` | Исходный входной поток. |
| load_options | `LoadOptions` | Параметры, включая пароль. |

### Пример

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # Откройте защищённый PDF как бинарный поток
    with open(r"C:\sample.pdf", "rb") as stream:
        # Укажите пароль через LoadOptions
        load_options = LoadOptions("mypassword")
        # Инициализируйте Redactor с потоком и параметрами загрузки
        with Redactor(stream, load_options) as redactor:
            # Выполните операции редактирования здесь
            pass
```

## __init__ {#document-load_options-settings}

Инициализирует новый экземпляр [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) для защищённого паролем документа, используя поток и настройки.

```python
def __init__(self, document, load_options, settings):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| document | `io.RawIOBase` | Исходный входной поток. |
| load_options | `LoadOptions` | Параметры, включая пароль. |
| settings | `RedactorSettings` | Настройки по умолчанию для процесса редактирования. |

### См. также
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
