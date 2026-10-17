---
title: "删除页面遮蔽"
linkTitle: "Remove page redactions"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "本文展示了如何从 PDF、演示文稿和电子表格文档中删除包含敏感数据的页面。"
type: docs
url: /zh/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction 可轻松删除 PDF 文档中的页面、演示文稿中的幻灯片以及电子表格文档中的工作表。

使用 GroupDocs.Redaction API，您可以通过指定页面范围的相对位置（开头或结尾）、零基索引以及要删除的页面数量来删除页面。目前支持的格式包括：PDF、演示文稿（Microsoft PowerPoint、OpenOffice 演示文稿）、文字处理文档（Microsoft Word、OpenOffice 文本、富文本文件）、电子表格（Microsoft Excel、OpenOffice 电子表格等）以及多帧图像。

## Remove page range

在下面的示例中，如果文档页数足够，我们将删除文档的第 2、3、4 页：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # 加载待编辑的文档
    with Redactor("./multipage_sample.pdf") as redactor:
        # 获取文档信息
        doc_info = redactor.get_document_info()

        # 至少需要 4 页
        if doc_info.page_count > 3:
            # 从第 2 页（零基索引 1）开始删除 3 页
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # 应用编辑
            result = redactor.apply(rem_opt)

            # 将脱敏后的文档保存到源文件旁边
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` 是本示例使用的示例文件。点击 [这里](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) 下载它。

## Remove last page

在某些情况下，您可能需要删除最后一页或若干页，无论文档有多少页。

以下示例演示如何从文档中删除最后一页：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # 从文档末尾计数删除 1 页
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # 加载待编辑的文档
    with Redactor("./multipage_sample.pdf") as redactor:
        # 获取文档信息
        doc_info = redactor.get_document_info()

        # 至少需要 2 页，以免文档为空
        if doc_info.page_count > 1:
            # 应用编辑
            result = redactor.apply(rem_opt)

            # 将脱敏后的文档保存到源文件旁边
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` 是本示例使用的示例文件。点击 [这里](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) 下载它。

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

对于多帧图像，您可能需要删除若干帧（视为"页面"）。

以下示例演示如何从动画 GIF 图像中删除 3 帧：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # 从第 3 帧（零基索引 2）开始删除帧
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # 加载待编辑的多帧图像
    with Redactor("./sample.gif") as redactor:
        # 获取文档信息
        doc_info = redactor.get_document_info()

        # 至少需要 7 帧
        if doc_info.page_count >= 7:
            # 应用编辑
            result = redactor.apply(rem_opt)

            # 将编辑后的图像保存到源文件旁边
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` 是本示例使用的示例文件。点击 [这里](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) 下载它。

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
