---
title: "метод save"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Сохраняет политику редактирования в файл."
type: docs
url: /ru/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Сохраняет политику редактирования в файл.

```python
def save(self, file_path):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| file_path | `str` | Путь к файлу. |

### Пример

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Сохраняет политику редактирования в поток.

```python
def save(self, output):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| output | `io.RawIOBase` | Целевой поток для сохранения политики. |

**Returns:** None.

### См. также
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
