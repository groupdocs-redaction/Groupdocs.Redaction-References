---
title: Redactor
second_title: .NET API 참조용 GroupDocs.Redaction
description: 문서 편집 프로세스를 제어하는 기본 클래스를 나타내며 문서를 열고 편집하고 저장할 수 있습니다.
type: docs
weight: 660
url: /ko/net/groupdocs.redaction/redactor/
---
## Redactor class

문서 편집 프로세스를 제어하는 기본 클래스를 나타내며 문서를 열고 편집하고 저장할 수 있습니다.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | 의 새 인스턴스를 초기화합니다.[`Redactor`](../redactor) stream. 를 사용하는 클래스 |
| [Redactor](redactor#constructor_3)(string) | 의 새 인스턴스를 초기화합니다.[`Redactor`](../redactor) 파일 경로를 사용하는 클래스. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | 의 새 인스턴스를 초기화합니다.[`Redactor`](../redactor) stream. 를 사용하는 암호로 보호된 문서의 클래스 |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | 의 새 인스턴스를 초기화합니다.[`Redactor`](../redactor) path. 를 사용하는 암호로 보호된 문서의 클래스 |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | 의 새 인스턴스를 초기화합니다.[`Redactor`](../redactor)스트림 및 설정을 사용하여 암호로 보호된 문서에 대한 클래스입니다. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | 의 새 인스턴스를 초기화합니다.[`Redactor`](../redactor) 경로와 설정을 사용하여 암호로 보호된 문서의 클래스. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | 문서에 교정을 적용합니다. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | 문서에 교정 정책을 적용합니다. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | 문서에 교정 세트를 적용합니다. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | 리소스를 해제합니다. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | 지정된 이미지 형식으로 특정 페이지의 미리보기 이미지를 생성합니다. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | 문서에 대한 일반 정보(크기, 페이지 수 등)를 가져옵니다. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | 다음 옵션을 사용하여 문서를 파일에 저장합니다. AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | 문서를 파일로 저장합니다. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | 사용자 지정 위치를 포함하여 문서를 스트림에 저장합니다. |

### 비고

**더 알아보기**

* 교정 적용에 대한 자세한 내용: [교정 기본 사항](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* 고급 편집 항목: [고급 사용법](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### 예

다음 예제는 단일 교정을 문서에 적용하는 방법을 보여줍니다.

다음 예제는 교정 목록을 문서에 적용하는 방법을 보여줍니다.

다음 예는 지정된 인바운드 폴더 내의 모든 파일에 수정 정책을 적용하고 성공적으로 업데이트된 파일과 실패한 파일에 대해 아웃바운드 폴더 중 하나에 저장하는 방법을 보여줍니다.

다음 예제에서는 LoadOptions를 사용하여 암호로 보호된 문서를 여는 방법을 보여줍니다.

다음 예제에서는 SaveOptions를 사용하여 문서를 저장하는 방법을 보여줍니다.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... 기타 교정
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // 적어도 하나의 편집이 실패한 경우 false
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // 여기에서 문서 인스턴스를 사용하여 교정을 수행할 수 있습니다.
}
```

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

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* 네임스페이스 [GroupDocs.Redaction](../../groupdocs.redaction)
* 집회 [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
