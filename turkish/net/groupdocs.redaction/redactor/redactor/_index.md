---
title: "Redactor"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Dosya yolu kullanarak Redactorgroupdocs.redaction/redactor sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Dosya yolu kullanarak [`Redactor`](../../redactor) sınıfının yeni bir örneğini başlatır.

```csharp
public Redactor(string filePath)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | String | Dosyanın yolu |

### Örnekler

Aşağıdaki örnek, bir belgeyi redaksiyon için nasıl açacağınızı gösterir.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Burada belge örneğini redaksiyonları gerçekleştirmek için kullanabiliriz
}
```

### Ayrıca Bakınız

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Akış kullanarak [`Redactor`](../../redactor) sınıfının yeni bir örneğini başlatır.

```csharp
public Redactor(Stream document)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| document | Akış | Belgenin kaynak akışı |

### Örnekler

Aşağıdaki örnek, bir belgeyi akıştan nasıl açacağınızı gösterir.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Burada belge örneğini redaksiyonları gerçekleştirmek için kullanabiliriz
    }
}
```

### Ayrıca Bakınız

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Şifre korumalı bir belge için yolunu kullanarak [`Redactor`](../../redactor) sınıfının yeni bir örneğini başlatır.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | String | Dosyanın yolu. |
| loadOptions | LoadOptions | Şifre dahil seçenekler. |

### Ayrıca Bakınız

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Şifre korumalı bir belge için yolunu ve ayarlarını kullanarak [`Redactor`](../../redactor) sınıfının yeni bir örneğini başlatır.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | String | Dosyanın yolu. |
| loadOptions | LoadOptions | Şifre dahil dosya bağımlı seçenekler. |
| settings | RedactorSettings | Kırpma işlemi için varsayılan ayarlar. |

### Ayrıca Bakınız

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Şifre korumalı bir belge için akışı kullanarak [`Redactor`](../../redactor) sınıfının yeni bir örneğini başlatır.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| document | Akış | Kaynak giriş akışı. |
| loadOptions | LoadOptions | Şifre dahil seçenekler. |

### Örnekler

Aşağıdaki örnek, LoadOptions kullanarak şifre korumalı belgelerin nasıl açılacağını gösterir.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Burada belge örneğini redaksiyonları gerçekleştirmek için kullanabiliriz
}
```

### Ayrıca Bakınız

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Akış ve ayarları kullanarak şifre korumalı bir belge için [`Redactor`](../../redactor) sınıfının yeni bir örneğini başlatır.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| document | Akış | Kaynak giriş akışı. |
| loadOptions | LoadOptions | Şifre dahil seçenekler. |
| settings | RedactorSettings | Kırpma işlemi için varsayılan ayarlar. |

### Örnekler

Aşağıdaki örnek, LoadOptions kullanarak şifre korumalı belgelerin nasıl açılacağını gösterir.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Burada belge örneğini redaksiyonları gerçekleştirmek için kullanabiliriz
}
```

### Ayrıca Bakınız

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
