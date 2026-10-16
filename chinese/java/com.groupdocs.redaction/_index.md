---
title: "com.groupdocs.redaction"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "该软件包提供用于从 PDF、光栅图像和办公文档格式的文档中编辑敏感信息的类。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.redaction/
---

该包提供用于从 PDF、光栅图像和办公文档格式的文档中编辑敏感信息的类。

该软件包中的主要类有：

<br />

* [Redactor](../../com.groupdocs.redaction/redactor) is the entry point for redaction process.
* [Redaction](../../com.groupdocs.redaction/redaction) is abstract base class for all types of document redactions.
* [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) is pre-configured in XML set of redaction rules.
* [RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) provides information about redaction process results.

<br />




## 类

| 类 | 描述 |
| --- | --- |
| [DocumentInfo](../com.groupdocs.redaction/documentinfo) | 表示有关文档的信息。 |
| [FileType](../com.groupdocs.redaction/filetype) | 表示一种文件类型。 |
| [PageInfo](../com.groupdocs.redaction/pageinfo) | 表示简要的页面信息。 |
| [Redaction](../com.groupdocs.redaction/redaction) | 表示所有编辑类型的基础抽象类。 |
| [RedactionPolicy](../com.groupdocs.redaction/redactionpolicy) | 表示一个清理策略，包含一组要应用的特定编辑。 |
| [RedactionResult](../com.groupdocs.redaction/redactionresult) | 表示编辑操作的结果。 |
| [Redactor](../com.groupdocs.redaction/redactor) | 表示控制文档编辑过程的主类，允许打开、编辑和保存文档。 |
| [RedactorChangeLog](../com.groupdocs.redaction/redactorchangelog) | 表示传递给 Redactor 类的 Apply() 方法的一系列编辑的结果。 |
| [RedactorLogEntry](../com.groupdocs.redaction/redactorlogentry) | 表示应用编辑的结果。 |

## 接口

| 接口 | 描述 |
| --- | --- |
| [IDocumentInfo](../com.groupdocs.redaction/idocumentinfo) | 定义获取基本文档信息所需的方法。 |

## 枚举

| 枚举 | 描述 |
| --- | --- |
| [RedactionStatus](../com.groupdocs.redaction/redactionstatus) | 表示编辑完成状态。 |
