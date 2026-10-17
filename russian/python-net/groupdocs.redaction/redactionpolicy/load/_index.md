---
title: "метод load"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Загружает RedactionPolicy из XML‑файла."
type: docs
url: /ru/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Загружает RedactionPolicy из XML‑файла.

```python
def load(cls, file_path):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| file_path | `str` | Путь к XML‑файлу. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Пример

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

Загружает экземпляр RedactionPolicy из потока, содержащего XML‑конфигурацию.

```python
def load(cls, input):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| input | `io.RawIOBase` | Поток, содержащий конфигурацию XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Пример

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Загрузить политику из XML‑файла
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Примените политику к документу
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### См. также
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
