---
title: "FileType"
second_title: "GroupDocs.Redaction for .NET API 참조"
description: "파일 유형을 나타냅니다. GroupDocs.Redaction에서 지원하는 모든 파일 유형 목록을 얻고, 확장자를 통해 파일 유형을 감지하는 등의 메서드를 제공합니다."
type: docs
weight: 90
url: /ko/net/groupdocs.redaction/filetype/
---
## FileType class

파일 형식을 나타냅니다. GroupDocs.Redaction에서 지원하는 모든 파일 형식 목록을 가져오고, 확장자를 통해 파일 형식을 감지하는 등의 메서드를 제공합니다.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | 비트맵 이미지 파일 (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | 쉼표로 구분된 값 파일 (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | DjVu 이미지 (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word 문서 (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML 매크로 사용 문서 (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML 문서 (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word 문서 템플릿 (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML 매크로 사용 문서 템플릿 (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML 문서 템플릿 (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | 그래픽 교환 형식 파일 (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | 하이퍼텍스트 마크업 언어 파일 (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | 하이퍼텍스트 마크업 언어 파일 (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 코어 이미지 파일 (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG 이미지 (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG 이미지 (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | 로그 파일 (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Markdown 문서 파일 (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers 스프레드시트 (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument 프레젠테이션 (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument 스프레드시트 (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument 텍스트 문서 (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | OpenDocument 프레젠테이션 템플릿 (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument 스프레드시트 템플릿 (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument 문서 템플릿 (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | 휴대용 문서 형식 파일 (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | 휴대용 네트워크 그래픽 (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | PowerPoint Open XML 매크로 사용 프레젠테이션 템플릿 (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | PowerPoint Open XML 프레젠테이션 템플릿 (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | PowerPoint 슬라이드 쇼 (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | PowerPoint Open XML 매크로 사용 슬라이드 (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | PowerPoint Open XML 슬라이드 쇼 (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint 프레젠테이션 (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | PowerPoint Open XML 매크로 사용 프레젠테이션 |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML 프레젠테이션 (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | 리치 텍스트 포맷 파일 (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | 탭 구분 값 파일 (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | 태그된 이미지 파일 (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | 태그된 이미지 파일 포맷 (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | 탭 구분 값 파일 (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | 일반 텍스트 파일 (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | 알 수 없는 파일 형식을 나타냅니다. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | WebP 이미지 (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel 스프레드시트 (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel 바이너리 스프레드시트 (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML 매크로 사용 스프레드시트 (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML 스프레드시트 (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Excel 템플릿 (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Excel Open XML 매크로 사용 스프레드시트 템플릿 (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Excel Open XML 스프레드시트 템플릿 (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | 파일 이름 접미사를 가져옵니다 (마침표 \".\" 포함), 예를 들어 \".doc\". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | 파일 형식 이름을 가져옵니다, 예를 들어 \"Microsoft Word Document\". |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | 파일 확장자를 파일 유형에 매핑합니다. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | 현재 [`FileType`](../filetype) 가 지정된 [`FileType`](../filetype) 객체와 동일한지 확인합니다. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | 현재 [`FileType`](../filetype) 가 지정된 객체와 동일한지 확인합니다. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | 현재 [`FileType`](../filetype) 객체의 해시 코드를 반환합니다. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | 현재 객체를 나타내는 문자열을 반환합니다. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | 지원되는 파일 유형을 검색합니다. |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | 두 [`FileType`](../filetype) 객체가 동일한지 확인합니다. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | 두 [`FileType`](../filetype) 객체가 동일하지 않은지 확인합니다. |

### 비고

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### 또 보기

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
