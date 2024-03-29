---
title: ImageAreaRedaction
second_title: GroupDocs.Redaction for .NET API 参考
description: 表示将彩色矩形放置在图像文档的给定区域中的编辑
type: docs
weight: 510
url: /zh/net/groupdocs.redaction.redactions/imagearearedaction/
---
## ImageAreaRedaction class

表示将彩色矩形放置在图像文档的给定区域中的编辑。

```csharp
public class ImageAreaRedaction : Redaction
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [ImageAreaRedaction](imagearearedaction)(Point, RegionReplacementOptions) | 初始化 ImageAreaRedaction 类的新实例，用于编辑特定区域大小。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/imagearearedaction/description) { get; } | 返回一个字符串，描述修订及其参数。 |
| [Options](../../groupdocs.redaction.redactions/imagearearedaction/options) { get; } | 获取[`RegionReplacementOptions`](../regionreplacementoptions)带有颜色和区域参数的选项. |
| [TopLeft](../../groupdocs.redaction.redactions/imagearearedaction/topleft) { get; } | 获取要移除的区域的左上角位置 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/imagearearedaction/applyto)(DocumentFormatInstance) | 将编辑应用到给定的格式实例。 |

### 评论

**了解更多**

* 有关应用密文的更多详细信息： [编辑基础知识](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* 有关图像编辑的更多详细信息： [图片编辑](https://docs.groupdocs.com/redaction/net/image-redactions/)

### 例子

以下示例演示用纯色矩形替换图像中的区域。

```csharp
    using (Redactor redactor = new Redactor("D:\\test.jpg"))
    {
       System.Drawing.Point samplePoint = new System.Drawing.Point(516, 311);
       System.Drawing.Size sampleSize = new System.Drawing.Size(170, 35);
       RedactorChangeLog result = redactor.Apply(new ImageAreaRedaction(samplePoint,
                     new RegionReplacementOptions(System.Drawing.Color.Blue, sampleSize)));
       if (result.Status != RedactionStatus.Failed)
       {
          redactor.Save();
       };
    } 
```

### 也可以看看

* class [Redaction](../../groupdocs.redaction/redaction)
* 命名空间 [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* 部件 [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
