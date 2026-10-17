---
title: "图像脱敏"
linkTitle: "Image redactions"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "本文展示了如何从 JPG、PNG、TIFF 等各种格式的图像中编辑敏感数据。"
type: docs
url: /zh/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions 提供了一套功能，可从 JPG、PNG、TIFF 等各种格式的图像中编辑敏感数据。请参阅 [supported document formats]() 文章获取完整列表。

GroupDocs.Redaction 支持两种图像编辑方式，分别是对独立图像文件和嵌入式图像进行编辑：
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

通过 .NET 的 GroupDocs.Redaction for Python 还允许您更改图像元数据（例如编辑图像的 EXIF 数据或充当“EXIF 擦除器”）。

## Redact image area

要编辑图像区域，您必须使用 [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) 类：

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # 定义要编辑区域的左上角位置
    sample_point = Point(385, 485)
    # 定义需要编辑的区域大小
    sample_size = Size(1793, 2069)
    # 定义编辑框的颜色
    color = Color.from_argb(255, 220, 20, 60)

    # 指定脱敏选项
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # 加载待编辑的文档
    with Redactor("./sample.jpg") as redactor:
        # 应用编辑
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # 默认情况下，已遮蔽的文档会以 PDF 格式保存
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` 是本示例使用的示例文件。点击 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) 下载。

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

如果无法对该类型的文件进行编辑，例如没有嵌入式图像的 MS Word 文档，则 [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) 将为 [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/)。

## Clean image metadata

下面的示例演示如何编辑（擦除）照片或其他图像的 EXIF 数据：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # 指定编辑选项以移除所有图像元数据（例如 EXIF）
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # 加载要编辑的图像
    with Redactor("./sample.jpg") as redactor:
        # 应用编辑
        result = redactor.apply(er_opt)

        # 将编辑后的图像保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` 是本示例使用的示例文件。点击 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) 下载。

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

如果无法对该类型的文件进行编辑，例如 BMP 图像，则 [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) 将为 [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/)。

## Redact embedded images

您可以对文档中所有类型的嵌入式图像的区域进行编辑。

下面的示例演示如何编辑 Microsoft Word 文档中所有嵌入的图像：

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # 定义要编辑区域的左上角位置
    sample_point = Point(516, 311)
    # 定义需要编辑的区域大小
    sample_size = Size(170, 35)
    # 定义编辑框的颜色
    color = Color.from_argb(255, 220, 20, 60)

    # 指定脱敏选项
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 对所有嵌入的图像应用编辑
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # 默认情况下，已遮蔽的文档会以 PDF 格式保存
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` 是本示例使用的示例文件。点击 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) 下载。

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

如果无法对该类型的文件进行编辑，例如电子表格文档，则 [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) 将为 [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/)。

## Multi-frame images

您可以使用指定的起始位置和帧计数从多帧图像中移除帧。更多信息请参阅 [remove page redactions]() 文章。

某些图像格式，例如 DjVu 文档，需要进行 [pre-rasterization]() 并进一步保存为 PDF 格式。
