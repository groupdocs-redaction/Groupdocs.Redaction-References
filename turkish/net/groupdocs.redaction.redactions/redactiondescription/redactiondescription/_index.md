---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "RedactionDescription sınıfının yeni bir örneğini, değiştirme bilgisi olmadan başlatır."
type: docs
weight: 10
url: /tr/net/groupdocs.redaction.redactions/redactiondescription/redactiondescription/
---
## RedactionDescription(RedactionType, RedactionActionType, string) {#constructor_1}

RedactionDescription sınıfının yeni bir örneğini, değiştirme bilgisi olmadan başlatır.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| redactionType | RedactionType | Silinen veri türü |
| actionType | RedactionActionType | Bu veriler üzerinde gerçekleştirilecek eylem |
| originalText | String | Eşleşen metin, yorum veya ek açıklama gövdesi |

### Ayrıca Bakınız

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, string, TextReplacement) {#constructor_2}

RedactionDescription sınıfının yeni bir örneğini, değiştirme bilgisiyle başlatır.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText, TextReplacement replacement)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| redactionType | RedactionType | Silinen veri türü |
| actionType | RedactionActionType | Bu veriler üzerinde gerçekleştirilecek eylem |
| originalText | String | Eşleşen metin, yorum veya ek açıklama gövdesi |
| replacement | TextReplacement | Değiştirme metni, eşleşen metin ve orijinal dizedeki konumu |

### Ayrıca Bakınız

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [TextReplacement](../../textreplacement)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, RegionReplacementOptions, string) {#constructor}

RedactionDescription sınıfının yeni bir örneğini, görüntü alanı değiştirme bilgisiyle başlatır.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    RegionReplacementOptions imageAreaReplacement, string imageDetails)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| redactionType | RedactionType | Silinen veri türü |
| actionType | RedactionActionType | Bu veriler üzerinde gerçekleştirilecek eylem |
| imageAreaReplacement | RegionReplacementOptions | Görüntü alanı değiştirme bilgisi |
| imageDetails | String | Görüntünün metinsel açıklaması, varsayılan olarak String.Empty'dir |

### Ayrıca Bakınız

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RegionReplacementOptions](../../regionreplacementoptions)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
