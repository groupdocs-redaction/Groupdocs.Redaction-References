---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Önizleme oluşturma için gereksinimleri ve stream delegelerini ayarlamak için seçenekler sağlar."
type: docs
weight: 11
url: /tr/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Önizleme oluşturma için gereksinimleri ve stream delegelerini ayarlamak için seçenekler sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | PreviewOptions sınıfının yeni bir örneğini başlatır, çıkış akışının kapanmasına neden olur. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | PreviewOptions sınıfının yeni bir örneğini başlatır, çıkış akışının daha sonraki kullanım için istemciye geri gönderilmesine neden olur. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getWidth()](#getWidth--) | Sayfa önizleme genişliğini alır veya ayarlar. |
|
|  | [setWidth(int value)](#setWidth-int-) | Sayfa önizleme genişliğini alır veya ayarlar. |
|
|  | [getHeight()](#getHeight--) | Sayfa önizleme yüksekliğini alır veya ayarlar. |
|
|  | [setHeight(int value)](#setHeight-int-) | Sayfa önizleme yüksekliğini alır veya ayarlar. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Önizleme oluşturulacak sayfa numaralarının bir dizisini alır veya ayarlar. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Önizleme oluşturulacak sayfa numaralarının bir dizisini alır veya ayarlar. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Önizleme görüntü formatını alır veya ayarlar. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Önizleme görüntü formatını alır veya ayarlar. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Sayfa akışı oluşturma temsilcisinin bir örneğini alır veya ayarlar. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Sayfa akışı oluşturma temsilcisinin bir örneğini alır veya ayarlar. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Sayfa önizleme tamamlama temsilcisinin bir örneğini alır veya ayarlar. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Sayfa önizleme tamamlama temsilcisinin bir örneğini alır veya ayarlar. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


PreviewOptions sınıfının yeni bir örneğini başlatır, çıkış akışının kapanmasına neden olur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Belirli bir sayfa önizlemesi için bir akış oluşturur |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


PreviewOptions sınıfının yeni bir örneğini başlatır, çıkış akışının daha sonraki kullanım için istemciye geri gönderilmesine neden olur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Belirli bir sayfa önizlemesi için bir akış oluşturur |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Sayfa önizleme oluşturmanın tamamlandığını bildirir ve çıkış akışını alır |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Sayfa önizleme genişliğini alır veya ayarlar.


**Returns:**
int - Sayfa önizleme genişliği.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Sayfa önizleme genişliğini alır veya ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Sayfa önizleme genişliği. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Sayfa önizleme yüksekliğini alır veya ayarlar.


**Returns:**
int - Sayfa önizleme yüksekliği.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Sayfa önizleme yüksekliğini alır veya ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Sayfa önizleme yüksekliği. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Önizleme oluşturulacak sayfa numaralarının bir dizisini alır veya ayarlar.


**Returns:**
int[] - Önizleme oluşturmak için sayfa numaralarının bir dizisi.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Önizleme oluşturulacak sayfa numaralarının bir dizisini alır veya ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int[] | Önizleme oluşturmak için sayfa numaralarının bir dizisi. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Önizleme görüntü formatını alır veya ayarlar.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Önizleme görüntü formatını alır veya ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Önizleme görüntü biçimi. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Sayfa akışı oluşturma temsilcisinin bir örneğini alır veya ayarlar.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Sayfa akışı oluşturma temsilcisinin bir örneğini alır veya ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Sayfa akışı oluşturma temsilcisinin bir örneği. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Sayfa önizleme tamamlama temsilcisinin bir örneğini alır veya ayarlar.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Sayfa önizleme tamamlama temsilcisinin bir örneğini alır veya ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Sayfa önizleme tamamlama temsilcisinin bir örneği. |
|

