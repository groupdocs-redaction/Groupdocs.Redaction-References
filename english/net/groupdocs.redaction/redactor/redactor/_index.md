---
title: Redactor
second_title: GroupDocs.Redaction for .NET API Reference
description: Initializes a new instance of Redactorgroupdocs.redaction/redactor class using file path.
type: docs
weight: 10
url: /net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Initializes a new instance of [`Redactor`](../../redactor) class using file path.

```csharp
public Redactor(string filePath)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | Path to the file |

### Examples

The following example demonstrates how to open a document for redaction.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Here we can use document instance to perform redactions
}
```

### See Also

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../redactor)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Initializes a new instance of [`Redactor`](../../redactor) class using stream.

```csharp
public Redactor(Stream document)
```

| Parameter | Type | Description |
| --- | --- | --- |
| document | Stream | Source stream of the document |

### Examples

The following example demonstrates how to open a document from stream.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Here we can use document instance to perform redactions
    }
}
```

### See Also

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../redactor)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Initializes a new instance of [`Redactor`](../../redactor) class for a password-protected document using its path.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | Path to file. |
| loadOptions | LoadOptions | Options, including password. |

### See Also

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../redactor)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Initializes a new instance of [`Redactor`](../../redactor) class for a password-protected document using its path and settings.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | Path to file. |
| loadOptions | LoadOptions | File-dependent options, including password. |
| settings | RedactorSettings | Default settings for redaction process. |

### See Also

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../redactor)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Initializes a new instance of [`Redactor`](../../redactor) class for a password-protected document using stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| document | Stream | Source input stream. |
| loadOptions | LoadOptions | Options, including password. |

### Examples

The following example demonstrates how to open a password-protected documents using LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Here we can use document instance to perform redactions
}
```

### See Also

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../redactor)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Initializes a new instance of [`Redactor`](../../redactor) class for a password-protected document using stream and settings.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Type | Description |
| --- | --- | --- |
| document | Stream | Source input stream. |
| loadOptions | LoadOptions | Options, including password. |
| settings | RedactorSettings | Default settings for redaction process. |

### Examples

The following example demonstrates how to open a password-protected documents using LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Here we can use document instance to perform redactions
}
```

### See Also

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../redactor)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.redaction.dll -->
