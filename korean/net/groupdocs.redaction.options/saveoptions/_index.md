---
title: SaveOptions
second_title: .NET API 참조용 GroupDocs.Redaction
description: 출력 파일 이름을 변경하거나 문서를 이미지 기반 PDF래스터화로 변환하기 위한 옵션을 제공합니다.
type: docs
weight: 380
url: /ko/net/groupdocs.redaction.options/saveoptions/
---
## SaveOptions class

출력 파일 이름을 변경하거나 문서를 이미지 기반 PDF(래스터화)로 변환하기 위한 옵션을 제공합니다.

```csharp
public class SaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | 기본값으로 새 인스턴스를 초기화합니다: PDF로 래스터화 - false, 접미사 추가 - false. |
| [SaveOptions](saveoptions#constructor_1)(bool, string) | 지정된 매개변수로 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AddSuffix](../../groupdocs.redaction.options/saveoptions/addsuffix) { get; set; } | 저장하기 전에 파일 이름을 변경해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. 기본적으로 거짓입니다. |
| [Rasterization](../../groupdocs.redaction.options/saveoptions/rasterization) { get; } | 래스터화 설정을 가져옵니다. |
| [RasterizeToPDF](../../groupdocs.redaction.options/saveoptions/rasterizetopdf) { get; set; } | 문서의 모든 페이지를 이미지로 변환하고 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [RedactedFileSuffix](../../groupdocs.redaction.options/saveoptions/redactedfilesuffix) { get; set; } | 출력 파일 이름에 대한 사용자 지정 접미사를 가져오거나 설정합니다. 지정되지 않은 경우,[`SaveSuffix`](./savesuffix) 상수가 사용됩니다. |

## 필드

| 이름 | 설명 |
| --- | --- |
| const [SaveSuffix](../../groupdocs.redaction.options/saveoptions/savesuffix) | "수정됨"인 기본 접미사 값을 나타냅니다. |

### 비고

**더 알아보기**

* [기본 옵션으로 저장](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
* [래스터화된 PDF로 저장](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* [래스터화된 PDF에 대한 특정 페이지 선택](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
* [원본 형식으로 저장](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
* [덮어쓰기 원본 파일 저장](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
* [스트림에 저장](https://docs.groupdocs.com/redaction/net/save-to-stream/)

### 예

다음 예제에서는 SaveOptions를 사용하여 문서를 저장하는 방법을 보여줍니다.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // 문서 편집은 여기로 이동합니다.
       // ...
    
       // 기본 옵션으로 문서 저장(페이지를 이미지로 변환, PDF로 저장)
       redactor.Save();
    
       // 원본 파일을 덮어써 원본 형식으로 문서 저장
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // 문서를 원본 형식으로 "*_Redacted.*" 파일에 저장
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // 문서를 래스터화하지 않고 파일 이름에 "*_AnyText.*"(예: "AnyText" 대신 타임스탬프)로 저장합니다.
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### 또한보십시오

* 네임스페이스 [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* 집회 [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
