---
title: "com.groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "该包提供用于将不同格式的文档与 GroupDocs.Redactions 集成的接口和类。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.redaction.integration/
---

该包提供用于将不同格式的文档与 GroupDocs.Redaction 集成的接口和类。



## 类

| 类 | 描述 |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | 表示文档的特定格式。 |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | 表示一个以标题为键的 MetadataItem 字典。 |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | 表示元数据项，适用于所有受支持的格式，并用于元数据编辑。 |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | 表示从图像中提取的文本，作为其识别过程的结果。 |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | 提供对所有光栅图像编辑操作的外观。 |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | 表示由 OCR 引擎提取的已识别文本的一部分（单词、符号等）。 |
| [TextLine](../com.groupdocs.redaction.integration/textline) | 表示由 OCR 引擎从图像中提取的一行文本。 |

## 接口

| 接口 | 描述 |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | 定义访问注释（如评论）所需的方法。 |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | 定义访问电子表格格式（具有一个或多个工作表）所需的方法。 |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | 定义访问固定结构格式（如 PDF 或演示文稿）所需的方法。 |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | 定义光栅图像格式编辑所需的方法。 |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | 定义访问文档元数据（如果格式支持）所需的方法。 |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | 定义一次使用相同颜色编辑多个图像区域所需的方法。 |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | 定义对图像文档和嵌入图像应用文本编辑所需的方法。 |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | 定义操作文档页面所需的方法。 |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | 定义创建文档预览的方法。 |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | 定义以任何二进制形式保存文档所需的方法。 |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | 定义在任何包含文本的文档中编辑文本数据所需的方法。 |
