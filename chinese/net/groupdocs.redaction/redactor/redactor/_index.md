---
title: Redactor
second_title: GroupDocs.Redaction for .NET API 参考
description: 初始化一个新实例Redactorgroupdocs.redaction/redactor使用文件路径的类.
type: docs
weight: 10
url: /zh/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

初始化一个新实例[`Redactor`](../../redactor)使用文件路径的类.

```csharp
public Redactor(string filePath)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径 |

### 例子

以下示例演示如何打开文档进行编辑。

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // 这里我们可以使用文档实例来执行编辑
}
```

### 也可以看看

* class [Redactor](../../redactor)
* 命名空间 [GroupDocs.Redaction](../../redactor)
* 部件 [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

初始化一个新实例[`Redactor`](../../redactor)使用 stream. 的类

```csharp
public Redactor(Stream document)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| document | Stream | 文档的源流 |

### 例子

以下示例演示如何从流中打开文档。

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // 这里我们可以使用文档实例来执行编辑
    }
}
```

### 也可以看看

* class [Redactor](../../redactor)
* 命名空间 [GroupDocs.Redaction](../../redactor)
* 部件 [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

初始化一个新实例[`Redactor`](../../redactor)使用其路径. 的受密码保护文档的类

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| loadOptions | LoadOptions | 选项，包括密码。 |

### 也可以看看

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* 命名空间 [GroupDocs.Redaction](../../redactor)
* 部件 [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

初始化一个新实例[`Redactor`](../../redactor)使用其路径和设置的受密码保护文档的类。

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| loadOptions | LoadOptions | 文件相关选项，包括密码。 |
| settings | RedactorSettings | 编辑过程的默认设置。 |

### 也可以看看

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* 命名空间 [GroupDocs.Redaction](../../redactor)
* 部件 [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

初始化一个新实例[`Redactor`](../../redactor)使用 stream. 的密码保护文档的类

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| document | Stream | 源输入流。 |
| loadOptions | LoadOptions | 选项，包括密码。 |

### 例子

下面的示例演示如何使用 LoadOptions 打开受密码保护的文件。

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // 这里我们可以使用文档实例来执行编辑
}
```

### 也可以看看

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* 命名空间 [GroupDocs.Redaction](../../redactor)
* 部件 [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

初始化一个新实例[`Redactor`](../../redactor)使用流和设置的密码保护文档的类。

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| document | Stream | 源输入流。 |
| loadOptions | LoadOptions | 选项，包括密码。 |
| settings | RedactorSettings | 编辑过程的默认设置。 |

### 例子

下面的示例演示如何使用 LoadOptions 打开受密码保护的文件。

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // 这里我们可以使用文档实例来执行编辑
}
```

### 也可以看看

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* 命名空间 [GroupDocs.Redaction](../../redactor)
* 部件 [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
