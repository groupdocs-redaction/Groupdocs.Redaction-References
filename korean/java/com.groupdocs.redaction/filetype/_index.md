---
title: "FileType"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "파일 유형을 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.redaction/filetype/
---
**Inheritance:**
java.lang.Object
```
public final class FileType
```

파일 유형을 나타냅니다. GroupDocs.Redaction에서 지원하는 모든 파일 유형 목록을 얻고, 확장자로 파일 유형을 감지하는 등의 메서드를 제공합니다.

*** ** * ** ***


**Learn more**

* [Supported Document Formats](../https://docs.groupdocs.com/redaction/java/supported-document-formats/)
* [Get supported file formats](../https://docs.groupdocs.com/redaction/java/get-supported-file-formats/)
* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | 예를 들어 "Microsoft Word Document"와 같은 파일 유형 이름을 가져옵니다. |
|
|  | [getExtension()](#getExtension--) | 파일명 접미사(점 "." 포함)를 가져옵니다. 예: ".doc". |
|
|  | [getUnknown()](#getUnknown--) | 알 수 없는 파일 유형을 나타냅니다. |
|
|  | [getTIF()](#getTIF--) | Tagged Image File (.tif) |
|
|  | [getTIFF()](#getTIFF--) | Tagged Image File Format (.tiff) |
|
|  | [getJPG()](#getJPG--) | JPEG 이미지 (.jpg) |
|
|  | [getJPEG()](#getJPEG--) | JPEG 이미지 (.jpeg) |
|
|  | [getPNG()](#getPNG--) | 포터블 네트워크 그래픽 (.png) |
|
|  | [getGIF()](#getGIF--) | 그래픽 교환 형식 파일 (.gif) |
|
|  | [getBMP()](#getBMP--) | 비트맵 이미지 파일 (.bmp) |
|
|  | [getJP2()](#getJP2--) | JPEG 2000 코어 이미지 파일 (.jp2) |
|
|  | [getHTM()](#getHTM--) | 하이퍼텍스트 마크업 언어 파일 (.htm) |
|
|  | [getHTML()](#getHTML--) | 하이퍼텍스트 마크업 언어 파일 (.html) |
|
|  | [getPDF()](#getPDF--) | 포터블 문서 형식 파일 (.pdf) |
|
|  | [getPPT()](#getPPT--) | PowerPoint 프레젠테이션 (.ppt) |
|
|  | [getPPTX()](#getPPTX--) | PowerPoint Open XML 프레젠테이션 (.pptx) |
|
|  | [getODP()](#getODP--) | OpenDocument 프레젠테이션 (.odp) |
|
|  | [getPOTX()](#getPOTX--) | PowerPoint Open XML 프레젠테이션 템플릿 (.potx) |
|
|  | [getPOTM()](#getPOTM--) | PowerPoint Open XML 매크로 사용 프레젠테이션 템플릿 (.potm) |
|
|  | [getOTP()](#getOTP--) | OpenDocument 프레젠테이션 템플릿 (.otp) |
|
|  | [getXLS()](#getXLS--) | Excel 스프레드시트 (.xls) |
|
|  | [getXLSX()](#getXLSX--) | Microsoft Excel Open XML 스프레드시트 (.xlsx) |
|
|  | [getXLSM()](#getXLSM--) | Excel Open XML 매크로 사용 스프레드시트 (.xlsm) |
|
|  | [getXLSB()](#getXLSB--) | Excel 바이너리 스프레드시트 (.xlsb) |
|
|  | [getXLTX()](#getXLTX--) | Excel Open XML 스프레드시트 템플릿 (.xltx) |
|
|  | [getXLTM()](#getXLTM--) | Excel Open XML 매크로 사용 스프레드시트 템플릿 (.xltm) |
|
|  | [getXLT()](#getXLT--) | Excel 템플릿 (.xlt) |
|
|  | [getCSV()](#getCSV--) | 쉼표 구분 값 파일 (.csv) |
|
|  | [getTSV()](#getTSV--) | 탭 구분 값 파일 (.tsv) |
|
|  | [getTAB()](#getTAB--) | 탭 구분 값 파일 (.tab) |
|
|  | [getODS()](#getODS--) | OpenDocument 스프레드시트 (.ods) |
|
|  | [getOTS()](#getOTS--) | OpenDocument 스프레드시트 템플릿 (.ots) |
|
|  | [getNUMBERS()](#getNUMBERS--) | Apple Numbers 스프레드시트 (.numbers) |
|
|  | [getMD()](#getMD--) | Markdown 문서 파일 (.md) |
|
|  | [getDOC()](#getDOC--) | Microsoft Word 문서 (.doc) |
|
|  | [getDOCX()](#getDOCX--) | Microsoft Word Open XML 문서 (.docx) |
|
|  | [getDOCM()](#getDOCM--) | Word Open XML 매크로 사용 문서 (.docm) |
|
|  | [getDOT()](#getDOT--) | Word 문서 템플릿 (.dot) |
|
|  | [getDOTX()](#getDOTX--) | Word Open XML 문서 템플릿 (.dotx) |
|
|  | [getDOTM()](#getDOTM--) | Word Open XML 매크로 사용 문서 템플릿 (.dotm) |
|
|  | [getRTF()](#getRTF--) | 리치 텍스트 포맷 파일 (.rtf) |
|
|  | [getTXT()](#getTXT--) | 일반 텍스트 파일 (.txt) |
|
|  | [getODT()](#getODT--) | OpenDocument 텍스트 문서 (.odt) |
|
|  | [getOTT()](#getOTT--) | OpenDocument 문서 템플릿 (.ott) |
|
|  | [fromExtension(String extension)](#fromExtension-java.lang.String-) | 파일 확장자를 파일 유형에 매핑합니다. |
|
|  | [getSupportedFileTypes()](#getSupportedFileTypes--) | 지원되는 파일 유형을 검색합니다 |
|
|  | [equals(FileType other)](#equals-com.groupdocs.redaction.FileType-) | 현재인지 여부를 판단합니다 |
FileType
지정된 것과 동일합니다
FileType
객체.
|
|  | [equals(Object obj)](#equals-java.lang.Object-) | 현재인지 여부를 판단합니다 |
FileType
지정된 객체와 동일합니다.
|
|  | [hashCode()](#hashCode--) | 현재에 대한 해시 코드를 반환합니다 |
FileType
객체.
|
|  | [op_Equality(FileType left, FileType right)](#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | 두 개가 동일한지 여부를 판단합니다 |
FileType
객체가 동일합니다.
|
|  | [op_Inequality(FileType left, FileType right)](#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-) | 두 개가 동일한지 여부를 판단합니다 |
FileType
객체가 동일하지 않습니다.
|
|  | [toString()](#toString--) | 현재 객체를 나타내는 문자열을 반환합니다. |
|
### getFileFormat() {#getFileFormat--}
```
public final String getFileFormat()
```


예를 들어 "Microsoft Word Document"와 같은 파일 유형 이름을 가져옵니다.


**Returns:**
java.lang.String - 파일 유형 이름, 예를 들어 "Microsoft Word Document".

### getExtension() {#getExtension--}
```
public final String getExtension()
```


파일명 접미사(점 "." 포함)를 가져옵니다. 예: ".doc".


**Returns:**
java.lang.String - 파일 이름 접미사(마침표 "." 포함), 예를 들어 ".doc".

### getUnknown() {#getUnknown--}
```
public static FileType getUnknown()
```


알 수 없는 파일 유형을 나타냅니다.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIF() {#getTIF--}
```
public static FileType getTIF()
```


Tagged Image File (.tif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTIFF() {#getTIFF--}
```
public static FileType getTIFF()
```


Tagged Image File Format (.tiff)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPG() {#getJPG--}
```
public static FileType getJPG()
```


JPEG 이미지 (.jpg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJPEG() {#getJPEG--}
```
public static FileType getJPEG()
```


JPEG 이미지 (.jpeg)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPNG() {#getPNG--}
```
public static FileType getPNG()
```


포터블 네트워크 그래픽 (.png)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getGIF() {#getGIF--}
```
public static FileType getGIF()
```


그래픽 교환 형식 파일 (.gif)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getBMP() {#getBMP--}
```
public static FileType getBMP()
```


비트맵 이미지 파일 (.bmp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getJP2() {#getJP2--}
```
public static FileType getJP2()
```


JPEG 2000 코어 이미지 파일 (.jp2)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTM() {#getHTM--}
```
public static FileType getHTM()
```


하이퍼텍스트 마크업 언어 파일 (.htm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getHTML() {#getHTML--}
```
public static FileType getHTML()
```


하이퍼텍스트 마크업 언어 파일 (.html)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPDF() {#getPDF--}
```
public static FileType getPDF()
```


포터블 문서 형식 파일 (.pdf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPT() {#getPPT--}
```
public static FileType getPPT()
```


PowerPoint 프레젠테이션 (.ppt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPPTX() {#getPPTX--}
```
public static FileType getPPTX()
```


PowerPoint Open XML 프레젠테이션 (.pptx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODP() {#getODP--}
```
public static FileType getODP()
```


OpenDocument 프레젠테이션 (.odp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTX() {#getPOTX--}
```
public static FileType getPOTX()
```


PowerPoint Open XML 프레젠테이션 템플릿 (.potx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getPOTM() {#getPOTM--}
```
public static FileType getPOTM()
```


PowerPoint Open XML 매크로 사용 프레젠테이션 템플릿 (.potm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTP() {#getOTP--}
```
public static FileType getOTP()
```


OpenDocument 프레젠테이션 템플릿 (.otp)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLS() {#getXLS--}
```
public static FileType getXLS()
```


Excel 스프레드시트 (.xls)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSX() {#getXLSX--}
```
public static FileType getXLSX()
```


Microsoft Excel Open XML 스프레드시트 (.xlsx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSM() {#getXLSM--}
```
public static FileType getXLSM()
```


Excel Open XML 매크로 사용 스프레드시트 (.xlsm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLSB() {#getXLSB--}
```
public static FileType getXLSB()
```


Excel 바이너리 스프레드시트 (.xlsb)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTX() {#getXLTX--}
```
public static FileType getXLTX()
```


Excel Open XML 스프레드시트 템플릿 (.xltx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLTM() {#getXLTM--}
```
public static FileType getXLTM()
```


Excel Open XML 매크로 사용 스프레드시트 템플릿 (.xltm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getXLT() {#getXLT--}
```
public static FileType getXLT()
```


Excel 템플릿 (.xlt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getCSV() {#getCSV--}
```
public static FileType getCSV()
```


쉼표 구분 값 파일 (.csv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTSV() {#getTSV--}
```
public static FileType getTSV()
```


탭 구분 값 파일 (.tsv)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTAB() {#getTAB--}
```
public static FileType getTAB()
```


탭 구분 값 파일 (.tab)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODS() {#getODS--}
```
public static FileType getODS()
```


OpenDocument 스프레드시트 (.ods)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTS() {#getOTS--}
```
public static FileType getOTS()
```


OpenDocument 스프레드시트 템플릿 (.ots)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getNUMBERS() {#getNUMBERS--}
```
public static FileType getNUMBERS()
```


Apple Numbers 스프레드시트 (.numbers)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getMD() {#getMD--}
```
public static FileType getMD()
```


Markdown 문서 파일 (.md)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOC() {#getDOC--}
```
public static FileType getDOC()
```


Microsoft Word 문서 (.doc)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCX() {#getDOCX--}
```
public static FileType getDOCX()
```


Microsoft Word Open XML 문서 (.docx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOCM() {#getDOCM--}
```
public static FileType getDOCM()
```


Word Open XML 매크로 사용 문서 (.docm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOT() {#getDOT--}
```
public static FileType getDOT()
```


Word 문서 템플릿 (.dot)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTX() {#getDOTX--}
```
public static FileType getDOTX()
```


Word Open XML 문서 템플릿 (.dotx)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getDOTM() {#getDOTM--}
```
public static FileType getDOTM()
```


Word Open XML 매크로 사용 문서 템플릿 (.dotm)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getRTF() {#getRTF--}
```
public static FileType getRTF()
```


리치 텍스트 포맷 파일 (.rtf)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getTXT() {#getTXT--}
```
public static FileType getTXT()
```


일반 텍스트 파일 (.txt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getODT() {#getODT--}
```
public static FileType getODT()
```


OpenDocument 텍스트 문서 (.odt)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### getOTT() {#getOTT--}
```
public static FileType getOTT()
```


OpenDocument 문서 템플릿 (.ott)


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype)
### fromExtension(String extension) {#fromExtension-java.lang.String-}
```
public static FileType fromExtension(String extension)
```


파일 확장자를 파일 유형에 매핑합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 확장자 | java.lang.String | 파일 확장자(마침표 "." 포함). |
|

**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - When file type is supported returns it, otherwise returns default  Unknown  file type.

### getSupportedFileTypes() {#getSupportedFileTypes--}
```
public static Iterable<FileType> getSupportedFileTypes()
```


지원되는 파일 유형을 검색합니다


**Returns:**
java.lang.Iterable<com.groupdocs.redaction.FileType> - 지원되는 파일 유형들의 시퀀스를 반환합니다

### equals(FileType other) {#equals-com.groupdocs.redaction.FileType-}
```
public final boolean equals(FileType other)
```


현재인지 여부를 판단합니다
FileType
지정된 것과 동일합니다
FileType
객체.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | other | [FileType](../../com.groupdocs.redaction/filetype) | 현재  FileType  객체와 비교할 객체. |
|

**Returns:**
boolean - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether the current 
FileType
 is the same as specified object.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with the current  FileType  object.
 |

**Returns:**
boolean - ```
true
```

if

```
obj
```

매개변수가  FileType 이며 현재  FileType  객체와 동일한 경우; 그렇지 않으면,

```
false
```


### hashCode() {#hashCode--}
```
public int hashCode()
```


현재에 대한 해시 코드를 반환합니다
FileType
객체.


**Returns:**
int - 현재  FileType  객체에 대한 해시 코드.

### op_Equality(FileType left, FileType right) {#op-Equality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Equality(FileType left, FileType right)
```


두 개가 동일한지 여부를 판단합니다
FileType
객체가 동일합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | left | [FileType](../../com.groupdocs.redaction/filetype) | 왼쪽  FileType  객체. |
|
|  | right | [FileType](../../com.groupdocs.redaction/filetype) | 오른쪽  FileType  객체. |
|

**Returns:**
boolean - ```
true
```

if both  FileType  objects are the same; otherwise,

```
false
```


### op_Inequality(FileType left, FileType right) {#op-Inequality-com.groupdocs.redaction.FileType-com.groupdocs.redaction.FileType-}
```
public static boolean op_Inequality(FileType left, FileType right)
```


Determines whether two 
FileType
 objects are not the same.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| left | [FileType](../../com.groupdocs.redaction/filetype) | Left  FileType  object.
 |
| right | [FileType](../../com.groupdocs.redaction/filetype) | Right  FileType  object.
 |

**Returns:**
boolean - ```
true
```

두  FileType  객체가 동일하지 않은 경우; 그렇지 않으면,

```
false
```


### toString() {#toString--}
```
public String toString()
```


현재 객체를 나타내는 문자열을 반환합니다.


**Returns:**
java.lang.String - 현재 객체를 나타내는 문자열.

