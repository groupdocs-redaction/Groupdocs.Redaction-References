---
title: "com.groupdocs.redaction.options"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "该包提供加载和保存选项类。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.redaction.options/
---

该包提供加载和保存选项类。



## 类

| 类 | 描述 |
| --- | --- |
| [LoadOptions](../com.groupdocs.redaction.options/loadoptions) | 提供用于打开文件的选项。 |
| [PreviewOptions](../com.groupdocs.redaction.options/previewoptions) | 提供用于设置预览生成的需求和流委托的选项。 |
| [RasterizationOptions](../com.groupdocs.redaction.options/rasterizationoptions) | 提供将文件转换为 PDF 的选项。 |
| [RedactorSettings](../com.groupdocs.redaction.options/redactorsettings) | 表示编辑设置，允许自定义编辑过程。 |
| [SaveOptions](../com.groupdocs.redaction.options/saveoptions) | 提供更改输出文件名和/或将文档转换为基于图像的 PDF（光栅化）的选项。 |
| [WordprocessingSaveOptions](../com.groupdocs.redaction.options/wordprocessingsaveoptions) | 文字处理保存选项。 |

## 接口

| 接口 | 描述 |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.redaction.options/icreatepagestream) | 提供返回用于写入页面预览数据的流的方法。 |
| [ILogger](../com.groupdocs.redaction.options/ilogger) | 定义可用于在编辑过程中记录事件和错误的日志记录器接口。 |
| [IReleasePageStream](../com.groupdocs.redaction.options/ireleasepagestream) | 表示释放由 CreatePageStream 委托创建的流的方法。 |

## 枚举

| 枚举 | 描述 |
| --- | --- |
| [AdvancedRasterizationOptions](../com.groupdocs.redaction.options/advancedrasterizationoptions) | 用于管理要应用的高级光栅化选项的枚举。 |
| [PdfComplianceLevel](../com.groupdocs.redaction.options/pdfcompliancelevel) | 表示受支持的 PDF 合规级别列表。 |
| [PreviewFormats](../com.groupdocs.redaction.options/previewformats) | 表示受支持的预览格式。 |
| [WordProcessingComplianceLevel](../com.groupdocs.redaction.options/wordprocessingcompliancelevel) | 文字处理文档的 OOXML 合规级别。 |
