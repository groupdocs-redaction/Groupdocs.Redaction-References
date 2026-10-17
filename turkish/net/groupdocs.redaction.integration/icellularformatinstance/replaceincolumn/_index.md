---
title: "ReplaceInColumn"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belirtilen sütun ve çalışma sayfasında tüm eşleşmeleri verilen bir değişiklikle değiştirir."
type: docs
weight: 20
url: /tr/net/groupdocs.redaction.integration/icellularformatinstance/replaceincolumn/
---
## ReplaceInColumn(Regex, string, int, int) {#replaceincolumn_1}

Belirtilen sütun ve çalışma sayfasında tüm eşleşmeleri verilen bir değişiklikle değiştirir.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column, 
    int sheet)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| regularExpression | Regex | Arama ve değiştirme için düzenli ifade |
| replacement | String | Metinsel değiştirme |
| column | Int32 | Sıfır tabanlı sütun indeksi |
| sayfa | Int32 | Sıfır tabanlı çalışma sayfası indeksi |

### Dönüş Değeri

Değiştirme sonucu

### Ayrıca Bakınız

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

---

## ReplaceInColumn(Regex, string, int) {#replaceincolumn}

Belirtilen sütunda tüm eşleşmeleri, tüm çalışma sayfalarında verilen bir değişiklikle değiştirir.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| regularExpression | Regex | Arama ve değiştirme için düzenli ifade |
| replacement | String | Metinsel değiştirme |
| column | Int32 | Sıfır tabanlı sütun indeksi |

### Dönüş Değeri

Değiştirme sonucu

### Ayrıca Bakınız

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
