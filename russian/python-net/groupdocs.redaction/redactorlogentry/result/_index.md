---
title: "свойство result"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Результат, возвращаемый DocumentFormatInstance."
type: docs
url: /ru/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

Результат, возвращаемый [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/).

Все редактирования метаданных применяются к каждому элементу метаданных отдельно, и даже если редактирование отдельного элемента метаданных не удалось, остальные элементы метаданных будут обновлены. Список неудачных, пропущенных (отклонённых) элементов метаданных и причины этого можно найти в свойстве `ErrorMessage` объекта [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

### Definition:
```python
@property
def result(self):
    ...
```

### См. также
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
