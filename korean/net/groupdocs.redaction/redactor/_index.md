---
title: "Redactor"
second_title: "GroupDocs.Redaction for .NET API 참조"
description: "문서 편집 프로세스를 제어하고 문서를 열고 편집하고 저장할 수 있는 주요 클래스를 나타냅니다."
type: docs
weight: 820
url: /ko/net/groupdocs.redaction/redactor/
---
## Redactor class

문서 리다크션 프로세스를 제어하는 주요 클래스를 나타내며, 문서를 열고, 리다크션하고, 저장할 수 있게 합니다.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | 스트림을 사용하여 [`Redactor`](../redactor) 클래스의 새 인스턴스를 초기화합니다. |
| [Redactor](redactor#constructor_3)(string) | 파일 경로를 사용하여 [`Redactor`](../redactor) 클래스의 새 인스턴스를 초기화합니다. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | 스트림을 사용하여 암호로 보호된 문서에 대한 [`Redactor`](../redactor) 클래스의 새 인스턴스를 초기화합니다. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | 경로를 사용하여 암호로 보호된 문서에 대해 [`Redactor`](../redactor) 클래스를 새 인스턴스로 초기화합니다. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | 스트림 및 설정을 사용하여 암호로 보호된 문서에 대해 [`Redactor`](../redactor) 클래스를 새 인스턴스로 초기화합니다. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | 경로와 설정을 사용하여 암호로 보호된 문서에 대해 [`Redactor`](../redactor) 클래스를 새 인스턴스로 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | 문서에 검열을 적용합니다. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | 문서에 검열 정책을 적용합니다. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | 문서에 일련의 검열을 적용합니다. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | 리소스를 해제합니다. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | 지정된 이미지 형식으로 특정 페이지의 미리보기 이미지를 생성합니다. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | 문서에 대한 일반 정보(크기, 페이지 수 등)를 가져옵니다. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | 다음 옵션을 사용하여 문서를 파일에 저장합니다: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | 문서를 파일에 저장합니다. |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | 문서를 지정된 스트림에 저장합니다. |

### 비고

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### 예제

다음 예제는 문서에 단일 검열을 적용하는 방법을 보여줍니다.

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

다음 예제는 문서에 검열 목록을 적용하는 방법을 보여줍니다.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... 기타 검열
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// 하나 이상의 검열이 실패한 경우 false
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

다음 예제는 지정된 인바운드 폴더 내 모든 파일에 리다크션 정책을 적용하고, 성공적으로 업데이트된 파일과 실패한 파일을 각각 아웃바운드 폴더에 저장하는 방법을 보여줍니다.

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

다음 예제는 LoadOptions를 사용하여 암호로 보호된 문서를 여는 방법을 보여줍니다.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // 여기서 문서 인스턴스를 사용하여 검열을 수행할 수 있습니다.
}
```

다음 예제는 SaveOptions를 사용하여 문서를 저장하는 방법을 보여줍니다.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // 문서 레드랙션이 여기 들어갑니다
       // ...
    
       // 기본 옵션으로 문서를 저장합니다 (페이지를 이미지로 변환하고 PDF로 저장)
       redactor.Save();
    
       // 원본 파일을 덮어쓰면서 원래 형식으로 문서를 저장합니다
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // 원래 형식으로 \"*_Redacted.*\" 파일에 문서를 저장합니다
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // 래스터화 없이 파일 이름에 \"*_AnyText.*\" (예: \"AnyText\" 대신 타임스탬프) 로 문서를 저장합니다
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### 또 보기

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
