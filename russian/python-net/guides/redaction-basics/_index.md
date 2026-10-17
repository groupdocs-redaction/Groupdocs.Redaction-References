---
title: "Основы редактирования"
linkTitle: "Redaction basics"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "В этой статье показано, как разработчики на Python могут применять редактирование метаданных, изображений, аннотаций и текста в своих документах. Поддерживается широкий спектр форматов документов, таких как PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX и другие."
type: docs
url: /ru/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction поддерживает эффективный набор функций редактирования документов. Он позволяет применять редактирование для [text](), [metadata](), [annotations](), [images]().

Поддерживается широкий спектр форматов документов, таких как: PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX и другие. Полный список поддерживаемых форматов см. в статье [supported document formats]().

## Redaction types

GroupDocs.Redaction поставляется со следующими типами редактирования:

| Тип | Описание | Классы |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

Применение редактирования к документу выполняется через метод [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) . В результате вы получаете экземпляр [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) , содержащий запись журнала для каждой применённой редактировки. Запись содержит ссылку на экземпляр [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) , включая его параметры, статус операции (см. ниже) и текстовые описания, если применимо. Если хотя бы одно редактирование завершилось с ошибкой, вы увидите [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) :

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Укажите параметры редактирования
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить редактирование
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Сохраните отредактированный документ рядом с исходным файлом
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) чтобы скачать его.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Все возможные статусы перечисления [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) перечислены в этой таблице:

| Статус | Описание | Возможные причины |
| --- | --- | --- |
| *Applied* | Редактирование было полностью и успешно применено | Все операции в процессе редактирования были успешно выполнены |
| *PartiallyApplied* | Редактирование было применено только к части совпадений | 1) Превышены ограничения пробной версии для замен 2) По крайней мере одно изменение было отклонено пользователем |
| *Skipped* | Редактирование было пропущено (не применено) | 1) Превышены ограничения пробной версии для редактирований 2) Редактирование невозможно применить к этому типу документа 3) Все замены были отклонены пользователем, и никаких изменений не внесено |
| *Failed* | Редактирование завершилось с ошибкой | Во время процесса редактирования возникло исключение |

Для получения подробной информации необходимо пройтись по записям журнала редактирования в [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) , и проверить свойство [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) у всех элементов со статусом, отличным от *Applied*:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # По умолчанию отредактированный документ сохраняется в формате PDF
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Сохранить все неудачные или пропущенные редактирования
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

Вы можете применить столько редактирований, сколько необходимо, одним вызовом метода [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) , поскольку его перегрузка принимает массив редактирований и политику редактирования. В этом случае редактирования будут применяться в том же порядке, в каком они указаны в массиве. В качестве альтернативы указанию наборов редактирований в коде, вы можете создать XML‑файл с политикой редактирования, как описано [здесь]().

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # Определите цвет блока редактирования
    color = Color.from_argb(255, 220, 20, 60)

    # Укажите список редактирований для применения в порядке их следования
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить список редактирований
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # По умолчанию отредактированный документ сохраняется в формате PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Сохранить все неудачные или пропущенные редактирования
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) чтобы скачать его.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
