---
title: ReplaceInColumn
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Belirtilen sütun ve çalışma sayfasındaki tüm eşleşmeleri belirli bir değiştirmeyle değiştirir.
type: docs
weight: 20
url: /tr/net/groupdocs.redaction.integration/icellularformatinstance/replaceincolumn/
---
## ReplaceInColumn(Regex, string, int, int) {#replaceincolumn_1}

Belirtilen sütun ve çalışma sayfasındaki tüm eşleşmeleri belirli bir değiştirmeyle değiştirir.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column, 
    int sheet)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| regularExpression | Regex | Aranacak ve değiştirilecek normal ifade |
| replacement | String | Metin değiştirme |
| column | Int32 | Sıfır tabanlı sütun dizini |
| sheet | Int32 | Sıfır tabanlı çalışma sayfası dizini |

### Geri dönüş değeri

Değiştirme sonucu

### Ayrıca bakınız

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* ad alanı [GroupDocs.Redaction.Integration](../../icellularformatinstance)
* toplantı [GroupDocs.Redaction](../../../)

---

## ReplaceInColumn(Regex, string, int) {#replaceincolumn}

Tüm eşleşmeleri, tüm çalışma sayfalarında belirtilen sütunda belirli bir değiştirme ile değiştirir.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| regularExpression | Regex | Aranacak ve değiştirilecek normal ifade |
| replacement | String | Metin değiştirme |
| column | Int32 | Sıfır tabanlı sütun dizini |

### Geri dönüş değeri

Değiştirme sonucu

### Ayrıca bakınız

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* ad alanı [GroupDocs.Redaction.Integration](../../icellularformatinstance)
* toplantı [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->