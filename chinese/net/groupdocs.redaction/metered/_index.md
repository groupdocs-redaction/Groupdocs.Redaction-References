---
title: Metered
second_title: GroupDocs.Redaction for .NET API 参考
description: 提供允许使用计量许可证激活产品并检索处理的 MB 数量的方法 了解有关计量许可证的更多信息这里https//purchase.groupdocs.com/faqs/licensing/metered.
type: docs
weight: 270
url: /zh/net/groupdocs.redaction/metered/
---
## Metered class

提供允许使用计量许可证激活产品并检索处理的 MB 数量的方法。 了解有关计量许可证的更多信息[这里](https://purchase.groupdocs.com/faqs/licensing/metered).

```csharp
public class Metered
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Metered](metered)() | 初始化 Metered 类的新实例。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | 使用计量密钥激活产品。 |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | 获取消费信用。 |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | 检索已处理的 MB 数量。 |

### 评论

**了解更多**

* 有关许可的更多信息： [GroupDocs 许可常见问题解答](https://purchase.groupdocs.com/faqs/licensing)
* 更多关于**GroupDocs.Redaction**许可： [评估限制和许可](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### 例子

以下示例演示了如何使用 Metered 密钥激活产品。

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

组件 jar 文件：

```csharp
Metered matered = new Metered();
matered.setMeteredKey("PublicKey", "PrivateKey");
```

### 也可以看看

* 命名空间 [GroupDocs.Redaction](../../groupdocs.redaction)
* 部件 [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
