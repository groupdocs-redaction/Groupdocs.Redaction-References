---
title: "RasterizationOptions 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "提供将文件转换为 PDF 的选项。"
type: docs
url: /zh/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

提供将文件转换为 PDF 的选项。

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

RasterizationOptions 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | 初始化新实例。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | 注册要应用的高级光栅化选项。 |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | 注册要应用的高级光栅化选项。 |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### 属性
| 属性 | 描述 |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | PDF 合规级别。 |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | 启用标志指示文档中的所有页面是否被转换为图像并放入单个 PDF 文件。默认值为 True；将其设为 False 可避免栅格化。 |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | 如果设置了高级栅格化选项，则指示器为 True。 |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | 要转换为 PDF 的页面数量。 |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | 要转换为 PDF 的第一页（从 0 开始计数）的索引。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### 另请参阅
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
