---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Uygulanacak belirli redaksiyonların bir kümesini içeren bir temizlik politikasını temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Uygulanacak belirli redaksiyonların bir kümesini içeren bir temizlik politikasını temsil eder.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Yeni bir Redaction politikası örneği oluşturur. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Belirli bir redaksiyon listesiyle yeni bir Redaction politikası örneği oluşturur. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Tamamen yapılandırılmış bir dizi alır |
Redaction
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Bir örnek yükler |
RedactionPolicy
dosya yolundan.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Bir örnek yükler |
RedactionPolicy
akıştan.
|
|  | [save(String filePath)](#save-java.lang.String-) | Redaction politikasını bir dosyaya kaydeder. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Redaction politikasını bir akışa kaydeder. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Yeni bir Redaction politikası örneği oluşturur.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Belirli bir redaksiyon listesiyle yeni bir Redaction politikası örneği oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Politika için bir redaksiyon dizisi |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Tamamen yapılandırılmış bir dizi alır
Redaction
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - Tamamen yapılandırılmış Redaction türevi sınıfların bir dizisi.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Bir örnek yükler
RedactionPolicy
dosya yolundan.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | XML dosyasının yolu |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Bir örnek yükler
RedactionPolicy
akıştan.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | girdi | java.io.InputStream | XML yapılandırmasını içeren akış |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Redaction politikasını bir dosyaya kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosya yolu. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Redaction politikasını bir akışa kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | çıktı | java.io.OutputStream | Politikayı kaydetmek için hedef akış |
|

