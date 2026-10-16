---
title: "TextRedaction"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili kelas abstrak dasar untuk redaksi teks dokumen."
type: docs
weight: 32
url: /id/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Mewakili kelas abstrak dasar untuk redaksi teks dokumen.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Mendapatkan |
ReplacementOptions
instansi, yang menentukan jenis penggantian teks.
|
|  | [getOcrConnector()](#getOcrConnector--) | Mendapatkan |
IOcrConnector
implementasi, diperlukan untuk mengekstrak teks dari konten grafis.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Mengatur |
IOcrConnector
implementasi, diperlukan untuk mengekstrak teks dari konten grafis.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Mendapatkan
ReplacementOptions
instansi, yang menentukan jenis penggantian teks.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Mendapatkan
IOcrConnector
implementasi, diperlukan untuk mengekstrak teks dari konten grafis.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Mengatur
IOcrConnector
implementasi, diperlukan untuk mengekstrak teks dari konten grafis.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Implementasi IOcrConnector, diperlukan untuk mengekstrak teks dari konten grafis. |
|

