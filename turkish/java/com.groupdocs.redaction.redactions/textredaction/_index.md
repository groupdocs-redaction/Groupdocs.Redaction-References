---
title: "TextRedaction"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Belge metni redaksiyonları için temel soyut bir sınıfı temsil eder."
type: docs
weight: 32
url: /tr/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Belge metni redaksiyonları için temel soyut bir sınıfı temsil eder.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Alır |
ReplacementOptions
örnek, metin değiştirme türünü belirten.
|
|  | [getOcrConnector()](#getOcrConnector--) | Alır |
IOcrConnector
uygulama, grafik içerikten metin çıkarmak için gereklidir.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Ayarlıyor |
IOcrConnector
uygulama, grafik içerikten metin çıkarmak için gereklidir.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Alır
ReplacementOptions
örnek, metin değiştirme türünü belirten.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Alır
IOcrConnector
uygulama, grafik içerikten metin çıkarmak için gereklidir.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Ayarlıyor
IOcrConnector
uygulama, grafik içerikten metin çıkarmak için gereklidir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector uygulaması, grafik içerikten metin çıkarmak için gereklidir. |
|

