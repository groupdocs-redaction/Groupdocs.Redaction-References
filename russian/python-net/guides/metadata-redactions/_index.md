---
title: "Редактирование метаданных"
linkTitle: "Metadata redactions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "В этой статье показано, как API редактирования Python позволяет заменять или удалять метаданные с помощью фильтров или поиска по регулярному выражению."
type: docs
url: /ru/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


С помощью API GroupDocs.Redaction вы можете применять редактирование метаданных к документам разных форматов, таких как PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX и другим. Смотрите полный список в статье [supported document formats]().

GroupDocs.Redactions предоставляет гибкий API, позволяющий заменять или удалять метаданные с помощью фильтров или поиска по регулярному выражению.

## Filter metadata

Базовая функциональность всех редактирований, наследующаяся от базового класса [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/), — это *metadata filtering* и она обязательна для редактирования метаданных. Она использует помечённую перечисление [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/), содержащее элементы для наиболее часто встречающихся записей метаданных. Вы можете установить фильтр на *All*, либо любую комбинацию метаданных. Например, нижеуказанный пример устанавливает фильтр на *Author*, *Manager* и *NameOfApplication* — для текстового редактирования или их очистки:

```python
# редактирование, основанное на MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

Ниже представлена таблица с полным списком элементов [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/):

| Фильтр | Числовое значение | Описание |
| --- | --- | --- |
| *None* | 0 | Пустая настройка фильтра, не соответствует ни одному элементу метаданных |
| *Author* | 1 | Автор документа |
| *Категория* | 2 | Категория документа |
| *Комментарии* | 4 | Комментарий к документу |
| *Компания* | 8 | Компания автора |
| *ContentStatus* | 16 | Состояние контента |
| *CreatedTime* | 32 | Время создания |
| *HyperlinkBase* | 64 | База гиперссылки |
| *LastPrinted* | 128 | Дата и время последней печати |
| *LastSavedBy* | 256 | Последнее сохранение пользователем |
| *LastSavedTime* | 1024 | Дата и время последнего сохранения |
| *NameOfApplication* | 2048 | Название приложения, в котором был создан документ |
| *Manager* | 4096 | Имя менеджера автора |
| *RevisionNumber* | 8192 | Номер ревизии |
| *Subject* | 16384 | Тема документа |
| *Template* | 32768 | Название шаблона документа |
| *Title* | 65536 | Заголовок документа |
| *TotalEditingTime* | 131072 | Общее время редактирования |
| *Версия* | 262144 | Версия документа |
| *Описание* | 524288 | Описание документа |
| *Ключевые слова* | 1048576 | Ключевые слова документа |
| *ContentType* | 2097152 | Тип содержимого |
| *Все* | 2147483647 | Все типы элементов метаданных |

## Clean metadata

Вы можете заменить все или отдельные метаданные в документе на пустые (пустые или минимальные) значения, используя класс [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/). Пример ниже очищает все свойства документа:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Укажите параметры редактирования, чтобы удалить все метаданные
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить редактирование
        result = redactor.apply(met_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx), чтобы скачать его.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

Вы можете указать [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) или использовать конструктор по умолчанию, чтобы очистить все метаданные в данном документе, Custom — чтобы удалить все пользовательские записи метаданных.

## Redact metadata

Вы можете использовать [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) для удаления конфиденциальных данных из метаданных документа с помощью регулярных выражений. Например, мы можем удалить любые упоминания "Company Ltd.":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Укажите параметры редактирования: шаблон поиска и строку замены
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить редактирование
        result = redactor.apply(met_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx), чтобы скачать его.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

Первый аргумент — регулярное выражение, второй — строка замены. Вы также можете задать область действия редактирования, установив фильтр, например, на [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). — это оставит совпадения регулярных выражений без изменений во всех элементах метаданных, кроме свойства "Company":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Укажите параметры редактирования: шаблон поиска и строку замены
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Ограничьте область редактирования только элементом метаданных Company
    met_red.filter = MetadataFilters.COMPANY

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить редактирование
        result = redactor.apply(met_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx), чтобы скачать его.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Все редактирования метаданных применяются к каждому элементу метаданных отдельно, и даже если редактирование элемента метаданных не удалось, остальные элементы будут обновлены. Список неудачных, пропущенных (отклонённых) элементов метаданных и причины можно найти в свойстве [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) объекта [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
