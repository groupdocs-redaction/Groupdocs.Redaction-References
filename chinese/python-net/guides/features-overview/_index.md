---
title: "功能概览"
linkTitle: "Features overview"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "通过 .NET 的 GroupDocs.Redaction for Python 使用单一、与格式无关的 API 删除文档中的敏感信息——文本、元数据、图像区域、批注和整页——并将结果保存为原始格式或已清理的 PDF。"
type: docs
url: /zh/python-net/guides/features-overview/
is_root: false
weight: 30
---


通过 .NET 的 GroupDocs.Redaction for Python 可在广泛的 [supported document formats]() 中删除或永久隐藏敏感信息。每次编辑都遵循相同的工作流：使用 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 打开文档，使用 `apply()` 应用一个或多个编辑，然后使用 `save()` 将清理后的结果保存为原始格式或已清理的 PDF。以下功能可以在一次处理过程中自由组合。

## Text redaction

通过精确短语或正则表达式查找并替换文本，覆盖完整单词以及诸如电子邮件地址、电话号码或国家身份证号码等复杂模式。匹配的文本可以替换为替代文本，或用彩色方框覆盖，使原始内容无法恢复。在电子表格中，您可以将搜索范围缩小到单个工作表或列。参见 [Text Redactions]().

## Metadata redaction

擦除或重写文档元数据——作者、标题、公司、注释以及图像的 EXIF 数据——以防止敏感细节通过文档属性泄露。您可以清除所有元数据、针对特定字段，或用新值替换。参见 [Metadata Redactions]().

## Image-area redaction

通过在给定区域绘制填充方框，将嵌入图像或扫描页的矩形区域涂黑——可用于隐藏签名、照片、页眉或页脚中可能出现的机密数据。参见 [Image Redactions]().

## Annotation redaction

重写或删除批注、评论和注释。您可以删除所有批注，或使用正则表达式仅匹配包含敏感文本的批注。参见 [Annotation Redactions]().

## Page removal

从 PDF 文档、演示文稿幻灯片和电子表格工作表中删除整页。您可以指定起始页和页数，并设定相对于起始点的方向。参见 [Remove Page Redactions]().

## Rasterization to PDF

将清理后的文档另存为页面渲染为光栅图像的 PDF。生成的文件不包含可搜索的文本，也不含原始元数据，因而被删除的内容无法恢复。光栅化是当您必须将文档交给第三方或遵守要求 PDF 的法规时的正确选择。您可以选择特定页面，并通过高级光栅化选项请求 PDF/A 合规。参见 [Save in Rasterized PDF]() 和 [Advanced Rasterization Options]().

## Redaction policies

将多个编辑标记组合成可重用的策略，并在众多文档中始终如一地应用相同规则——非常适合在发布前清除标准字段等重复任务。参见 [Use Redaction Policies]().

## Loading and saving

从本地路径或流加载文档，包括受密码保护的文件，并可在编辑前预先光栅化文档。保存时，可保持原始格式以便进一步编辑，覆盖原文件，光栅化为 PDF，或写入流。参见 [Loading Documents]() 和 [Saving Documents]().

## On-premise

GroupDocs.Redaction for Python via .NET 完全在您自己的基础设施上运行——文档永不离开您的环境。该包是一个自包含的 wheel，捆绑所有必需内容，无需安装 Microsoft Office、OpenOffice、Adobe Acrobat 或其他运行时。参见 [System Requirements]() 了解受支持的平台和本机依赖项。
