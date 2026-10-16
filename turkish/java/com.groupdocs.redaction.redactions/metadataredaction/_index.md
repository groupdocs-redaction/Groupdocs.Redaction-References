---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Belge meta verisi redaksiyonları için temel soyut bir sınıfı temsil eder."
type: docs
weight: 20
url: /tr/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Belge meta verisi redaksiyonları için temel soyut bir sınıfı temsil eder.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFilter()](#getFilter--) | Tüm veya belirli meta verileri seçmek için kullanılan filtreyi alır, örneğin Yazar veya Şirket. |
|
|  | [setFilter(int value)](#setFilter-int-) | Tüm veya belirli meta verileri seçmek için kullanılan filtreyi ayarlar, örneğin Yazar veya Şirket. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Redaksiyonu verilen format örneğine uygular. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Tüm veya belirli meta verileri seçmek için kullanılan filtreyi alır, örneğin Yazar veya Şirket.


**Returns:**
int - Tüm veya belirli meta verileri seçmek için kullanılan filtre, örneğin Yazar ve Şirket.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Tüm veya belirli meta verileri seçmek için kullanılan filtreyi ayarlar, örneğin Yazar veya Şirket.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Tüm veya belirli meta verileri seçmek için kullanılan filtre, örneğin Yazar ve Şirket. |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Redaksiyonu verilen format örneğine uygular.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Redaksiyon uygulamak için bir belge örneği |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

