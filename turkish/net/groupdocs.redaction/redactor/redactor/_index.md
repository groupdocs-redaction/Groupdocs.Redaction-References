---
title: Redactor
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Yeni bir örneğini başlatırRedactorgroupdocs.redaction/redactor dosya yolunu kullanan sınıf.
type: docs
weight: 10
url: /tr/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Yeni bir örneğini başlatır[`Redactor`](../../redactor) dosya yolunu kullanan sınıf.

```csharp
public Redactor(string filePath)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | dosyanın yolu |

### Örnekler

Aşağıdaki örnek, bir belgenin redaksiyon için nasıl açılacağını gösterir.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Burada redaksiyon yapmak için belge örneğini kullanabiliriz
}
```

### Ayrıca bakınız

* class [Redactor](../../redactor)
* ad alanı [GroupDocs.Redaction](../../redactor)
* toplantı [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Yeni bir örneğini başlatır[`Redactor`](../../redactor) stream. kullanan sınıf

```csharp
public Redactor(Stream document)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| document | Stream | Belgenin kaynak akışı |

### Örnekler

Aşağıdaki örnek, akıştan bir belgenin nasıl açılacağını gösterir.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Burada redaksiyon yapmak için belge örneğini kullanabiliriz
    }
}
```

### Ayrıca bakınız

* class [Redactor](../../redactor)
* ad alanı [GroupDocs.Redaction](../../redactor)
* toplantı [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Yeni bir örneğini başlatır[`Redactor`](../../redactor) path. kullanan parola korumalı bir belge için sınıf

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosya yolu. |
| loadOptions | LoadOptions | Parola dahil seçenekler. |

### Ayrıca bakınız

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* ad alanı [GroupDocs.Redaction](../../redactor)
* toplantı [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Yeni bir örneğini başlatır[`Redactor`](../../redactor) yolunu ve ayarlarını kullanan parola korumalı bir belge için sınıf.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosya yolu. |
| loadOptions | LoadOptions | Parola dahil dosyaya bağlı seçenekler. |
| settings | RedactorSettings | Düzeltme işlemi için varsayılan ayarlar. |

### Ayrıca bakınız

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* ad alanı [GroupDocs.Redaction](../../redactor)
* toplantı [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Yeni bir örneğini başlatır[`Redactor`](../../redactor) stream. kullanan parola korumalı bir belge için sınıf

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| document | Stream | Kaynak giriş akışı. |
| loadOptions | LoadOptions | Parola dahil seçenekler. |

### Örnekler

Aşağıdaki örnek, parola korumalı belgelerin LoadOptions kullanılarak nasıl açılacağını gösterir.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Burada redaksiyon yapmak için belge örneğini kullanabiliriz
}
```

### Ayrıca bakınız

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* ad alanı [GroupDocs.Redaction](../../redactor)
* toplantı [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Yeni bir örneğini başlatır[`Redactor`](../../redactor)akış ve ayarları kullanan parola korumalı bir belge için sınıf.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| document | Stream | Kaynak giriş akışı. |
| loadOptions | LoadOptions | Parola dahil seçenekler. |
| settings | RedactorSettings | Düzeltme işlemi için varsayılan ayarlar. |

### Örnekler

Aşağıdaki örnek, parola korumalı belgelerin LoadOptions kullanılarak nasıl açılacağını gösterir.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Burada redaksiyon yapmak için belge örneğini kullanabiliriz
}
```

### Ayrıca bakınız

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* ad alanı [GroupDocs.Redaction](../../redactor)
* toplantı [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
