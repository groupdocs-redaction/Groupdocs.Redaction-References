---
title: "Редактирование изображений"
linkTitle: "Image redactions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "В этой статье показано, как удалять конфиденциальные данные из изображений различных форматов, таких как JPG, PNG, TIFF и другие."
type: docs
url: /ru/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions предоставляет набор функций для удаления конфиденциальных данных из изображений различных форматов, таких как JPG, PNG, TIFF и другие. Полный список см. в статье [supported document formats]().

GroupDocs.Redaction поддерживает два способа редактирования изображений: как в отдельных файлах изображений, так и во встроенных изображениях:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction for Python via .NET также позволяет вам изменять метаданные изображений (например, редактировать EXIF‑данные изображения или выступать в роли «стерки EXIF»).

## Redact image area

Чтобы удалить область изображения, вам необходимо использовать класс [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Укажите позицию верхнего левого угла области для удаления
    sample_point = Point(385, 485)
    # Укажите размер области, которую необходимо удалить
    sample_size = Size(1793, 2069)
    # Определите цвет блока редактирования
    color = Color.from_argb(255, 220, 20, 60)

    # Укажите параметры редактирования
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./sample.jpg") as redactor:
        # Применить редактирование
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # По умолчанию отредактированный документ сохраняется в формате PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg), чтобы скачать его.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Если удаление не может быть применено к этому типу файлов, например к документу MS Word без встроенных изображений, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) будет иметь значение [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Clean image metadata

В следующем примере показано, как редактировать EXIF‑данные (стереть их) из фотографии или любого другого изображения:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Укажите параметры удаления, чтобы удалить все метаданные изображения (например, EXIF)
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Загрузите изображение, которое нужно удалить
    with Redactor("./sample.jpg") as redactor:
        # Применить редактирование
        result = redactor.apply(er_opt)

        # Сохранить отредактированное изображение рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg), чтобы скачать его.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Если удаление не может быть применено к этому типу файлов, например к BMP‑изображению, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) будет иметь значение [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Redact embedded images

Вы можете удалять области изображений во всех типах встроенных изображений внутри документа.

В следующем примере показано, как удалить все встроенные изображения в документе Microsoft Word:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Укажите позицию верхнего левого угла области для удаления
    sample_point = Point(516, 311)
    # Укажите размер области, которую необходимо удалить
    sample_size = Size(170, 35)
    # Определите цвет блока редактирования
    color = Color.from_argb(255, 220, 20, 60)

    # Укажите параметры редактирования
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Примените удаление ко всем встроенным изображениям
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # По умолчанию отредактированный документ сохраняется в формате PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx), чтобы скачать его.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Если удаление не может быть применено к этому типу файлов, например к таблице, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) будет иметь значение [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Multi-frame images

Вы можете удалять кадры из многокадрового изображения, указав исходную позицию и количество кадров. Для дополнительной информации см. статью [remove page redactions]().

Некоторые форматы изображений, такие как документы DjVu, требуют [pre-rasterization]() и последующего сохранения в формате PDF.
