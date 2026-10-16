---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "미리보기 생성을 위한 요구 사항 및 스트림 대리자를 설정하는 옵션을 제공합니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

미리보기 생성을 위한 요구 사항 및 스트림 대리자를 설정하는 옵션을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | PreviewOptions 클래스의 새 인스턴스를 초기화하고, 출력 스트림이 닫히도록 합니다. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | PreviewOptions 클래스의 새 인스턴스를 초기화하고, 출력 스트림이 클라이언트에 반환되어 이후에 사용할 수 있도록 합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getWidth()](#getWidth--) | 페이지 미리보기 너비를 가져오거나 설정합니다. |
|
|  | [setWidth(int value)](#setWidth-int-) | 페이지 미리보기 너비를 가져오거나 설정합니다. |
|
|  | [getHeight()](#getHeight--) | 페이지 미리보기 높이를 가져오거나 설정합니다. |
|
|  | [setHeight(int value)](#setHeight-int-) | 페이지 미리보기 높이를 가져오거나 설정합니다. |
|
|  | [getPageNumbers()](#getPageNumbers--) | 미리보기를 생성할 페이지 번호 배열을 가져오거나 설정합니다. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | 미리보기를 생성할 페이지 번호 배열을 가져오거나 설정합니다. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | 미리보기 이미지 형식을 가져오거나 설정합니다. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | 미리보기 이미지 형식을 가져오거나 설정합니다. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | 페이지 스트림 생성 대리자 인스턴스를 가져오거나 설정합니다. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | 페이지 스트림 생성 대리자 인스턴스를 가져오거나 설정합니다. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | 페이지 미리보기 완료 대리자 인스턴스를 가져오거나 설정합니다. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | 페이지 미리보기 완료 대리자 인스턴스를 가져오거나 설정합니다. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


PreviewOptions 클래스의 새 인스턴스를 초기화하고, 출력 스트림이 닫히도록 합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | 특정 페이지 미리보기를 위한 스트림을 생성합니다. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


PreviewOptions 클래스의 새 인스턴스를 초기화하고, 출력 스트림이 클라이언트에 반환되어 이후에 사용할 수 있도록 합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | 특정 페이지 미리보기를 위한 스트림을 생성합니다. |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | 페이지 미리보기 생성이 완료되었음을 알리고 출력 스트림을 가져옵니다. |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


페이지 미리보기 너비를 가져오거나 설정합니다.


**Returns:**
int - 페이지 미리보기 너비.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


페이지 미리보기 너비를 가져오거나 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | 페이지 미리보기 너비. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


페이지 미리보기 높이를 가져오거나 설정합니다.


**Returns:**
int - 페이지 미리보기 높이.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


페이지 미리보기 높이를 가져오거나 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | 페이지 미리보기 높이. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


미리보기를 생성할 페이지 번호 배열을 가져오거나 설정합니다.


**Returns:**
int[] - 미리보기를 생성할 페이지 번호 배열.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


미리보기를 생성할 페이지 번호 배열을 가져오거나 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int[] | 미리보기를 생성할 페이지 번호 배열. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


미리보기 이미지 형식을 가져오거나 설정합니다.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


미리보기 이미지 형식을 가져오거나 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | 미리보기 이미지 형식. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


페이지 스트림 생성 대리자 인스턴스를 가져오거나 설정합니다.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


페이지 스트림 생성 대리자 인스턴스를 가져오거나 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | 페이지 스트림 생성 대리자 인스턴스. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


페이지 미리보기 완료 대리자 인스턴스를 가져오거나 설정합니다.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


페이지 미리보기 완료 대리자 인스턴스를 가져오거나 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | 페이지 미리보기 완료 대리자 인스턴스. |
|

