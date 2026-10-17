---
title: "Редактирование аннотаций"
linkTitle: "Annotation redactions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "В этой статье показана реализация редактирования аннотаций для документов разных форматов, таких как PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX и других."
type: docs
url: /ru/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


С помощью API GroupDocs.Redaction вы можете применять редактирование аннотаций к документам разных форматов, таких как PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX и другие. Полный список см. в статье [supported document formats]().

GroupDocs.Redactions предоставляет гибкий API, позволяющий удалять конфиденциальные данные из текста аннотации или полностью удалять аннотации с помощью регулярного выражения.

## Remove annotations (comments etc)

Вы можете использовать GroupDocs.Redaction для удаления всех или определённых комментариев и других аннотаций из документа. Например, можно удалить все комментарии из документа, содержащие такие тексты, как "use", "show" или "describe" в их содержании:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Укажите параметры редактирования для удаления аннотаций, соответствующих шаблону
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Загрузите документ для редактирования
    with Redactor("./annotated.xlsx") as redactor:
        # Применить редактирование
        result = redactor.apply(a_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` — пример файла, используемый в этом примере. Нажмите [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx), чтобы скачать его.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

Вы можете использовать конструктор без аргументов, чтобы удалить все аннотации в документе.

## Redact annotations

Вместо удаления всех или конкретных аннотаций, вы можете удалить конфиденциальные данные из текста аннотации. Например, мы можем удалить все упоминания "John" в данном документе, например:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Укажите параметры редактирования: шаблон поиска и строку замены
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Загрузите документ для редактирования
    with Redactor("./annotated.xlsx") as redactor:
        # Применить редактирование
        result = redactor.apply(a_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` — пример файла, используемый в этом примере. Нажмите [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx), чтобы скачать его.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
