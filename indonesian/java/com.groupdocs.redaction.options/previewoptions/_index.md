---
title: "PreviewOptions"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Menyediakan opsi untuk mengatur persyaratan dan delegasi aliran untuk pembuatan pratinjau."
type: docs
weight: 11
url: /id/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Menyediakan opsi untuk mengatur persyaratan dan delegasi aliran untuk pembuatan pratinjau.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Menginisialisasi sebuah instance baru dari kelas PreviewOptions, yang menyebabkan aliran keluaran ditutup. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Menginisialisasi sebuah instance baru dari kelas PreviewOptions, yang menyebabkan aliran keluaran dikembalikan ke klien untuk penggunaan lebih lanjut. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getWidth()](#getWidth--) | Mendapatkan atau mengatur lebar pratinjau halaman. |
|
|  | [setWidth(int value)](#setWidth-int-) | Mendapatkan atau mengatur lebar pratinjau halaman. |
|
|  | [getHeight()](#getHeight--) | Mendapatkan atau mengatur tinggi pratinjau halaman. |
|
|  | [setHeight(int value)](#setHeight-int-) | Mendapatkan atau mengatur tinggi pratinjau halaman. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Mendapatkan atau mengatur array nomor halaman untuk menghasilkan pratinjau. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Mendapatkan atau mengatur array nomor halaman untuk menghasilkan pratinjau. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Mendapatkan atau mengatur format gambar pratinjau. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Mendapatkan atau mengatur format gambar pratinjau. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Mendapatkan atau mengatur instance delegasi pembuatan aliran halaman. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Mendapatkan atau mengatur instance delegasi pembuatan aliran halaman. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Mendapatkan atau mengatur instance delegasi penyelesaian pratinjau halaman. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Mendapatkan atau mengatur instance delegasi penyelesaian pratinjau halaman. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Menginisialisasi sebuah instance baru dari kelas PreviewOptions, yang menyebabkan aliran keluaran ditutup.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Membuat aliran untuk pratinjau halaman tertentu |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Menginisialisasi sebuah instance baru dari kelas PreviewOptions, yang menyebabkan aliran keluaran dikembalikan ke klien untuk penggunaan lebih lanjut.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Membuat aliran untuk pratinjau halaman tertentu |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Memberitahukan bahwa pembuatan pratinjau halaman selesai dan mendapatkan aliran output |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Mendapatkan atau mengatur lebar pratinjau halaman.


**Returns:**
int - Lebar pratinjau halaman.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Mendapatkan atau mengatur lebar pratinjau halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Lebar pratinjau halaman. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Mendapatkan atau mengatur tinggi pratinjau halaman.


**Returns:**
int - Tinggi pratinjau halaman.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Mendapatkan atau mengatur tinggi pratinjau halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Tinggi pratinjau halaman. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Mendapatkan atau mengatur array nomor halaman untuk menghasilkan pratinjau.


**Returns:**
int[] - Array nomor halaman untuk menghasilkan pratinjau.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Mendapatkan atau mengatur array nomor halaman untuk menghasilkan pratinjau.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int[] | Array nomor halaman untuk menghasilkan pratinjau. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Mendapatkan atau mengatur format gambar pratinjau.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Mendapatkan atau mengatur format gambar pratinjau.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Format gambar pratinjau. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Mendapatkan atau mengatur instance delegasi pembuatan aliran halaman.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Mendapatkan atau mengatur instance delegasi pembuatan aliran halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Instance delegasi pembuatan aliran halaman. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Mendapatkan atau mengatur instance delegasi penyelesaian pratinjau halaman.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Mendapatkan atau mengatur instance delegasi penyelesaian pratinjau halaman.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Instance delegasi penyelesaian pratinjau halaman. |
|

