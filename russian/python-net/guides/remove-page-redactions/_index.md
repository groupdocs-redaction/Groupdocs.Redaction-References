---
title: "Удалить редактирование страниц"
linkTitle: "Remove page redactions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "В этой статье показано, как удалить страницы с конфиденциальными данными из ваших PDF, презентаций и таблиц."
type: docs
url: /ru/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction позволяет легко удалять страницы из PDF‑документов, слайды из презентаций и листы из электронных таблиц.

С помощью GroupDocs.Redaction API вы можете удалять страницы, указывая диапазон страниц с помощью их относительного положения (начало или конец), нулевого индекса и количества страниц для удаления. На данный момент поддерживаемые форматы: PDF, презентации (Microsoft PowerPoint, OpenOffice Presentations), текстовые документы (Microsoft Word, OpenOffice Texts, Rich Text Files), электронные таблицы (Microsoft Excel, OpenOffice Spreadsheets и др.) и многокадровые изображения.

## Remove page range

В приведённом ниже примере мы удаляем 2‑ю, 3‑ю и 4‑ю страницы из документа, если в документе достаточно страниц:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Загрузите документ для редактирования
    with Redactor("./multipage_sample.pdf") as redactor:
        # Получить информацию о документе
        doc_info = redactor.get_document_info()

        # Требуется минимум 4 страницы
        if doc_info.page_count > 3:
            # Удалить 3 страницы, начиная со второй (ноль‑базовый индекс 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Применить редактирование
            result = redactor.apply(rem_opt)

            # Сохраните отредактированный документ рядом с исходным файлом
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) для его загрузки.

## Remove last page

В некоторых случаях вам может потребоваться удалить последнюю страницу или несколько страниц, независимо от их количества.

В следующем примере показано, как удалить последнюю страницу из документа:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Удалить 1 страницу, считая от конца документа
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Загрузите документ для редактирования
    with Redactor("./multipage_sample.pdf") as redactor:
        # Получить информацию о документе
        doc_info = redactor.get_document_info()

        # Требуется минимум 2 страницы, чтобы документ не оказался пустым
        if doc_info.page_count > 1:
            # Применить редактирование
            result = redactor.apply(rem_opt)

            # Сохраните отредактированный документ рядом с исходным файлом
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) для его загрузки.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

В случае многокадрового изображения вам может потребоваться удалить несколько кадров (рассматриваемых как "страницы").

В следующем примере показано, как удалить 3 кадра из анимированного GIF‑изображения:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # Удалить кадры, начиная с третьего (ноль‑базовый индекс 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Загрузить многокадровое изображение для редактирования
    with Redactor("./sample.gif") as redactor:
        # Получить информацию о документе
        doc_info = redactor.get_document_info()

        # Требуется минимум 7 кадров
        if doc_info.page_count >= 7:
            # Применить редактирование
            result = redactor.apply(rem_opt)

            # Сохранить отредактированное изображение рядом с исходным файлом
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) для его загрузки.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
