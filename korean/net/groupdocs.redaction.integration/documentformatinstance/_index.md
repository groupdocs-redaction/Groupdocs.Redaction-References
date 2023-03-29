---
title: DocumentFormatInstance
second_title: .NET API 참조용 GroupDocs.Redaction
description: 문서의 특정 형식을 나타냅니다. 자신의 문서 유형을 추가하려면 이 클래스를 구현하십시오.
type: docs
weight: 110
url: /ko/net/groupdocs.redaction.integration/documentformatinstance/
---
## DocumentFormatInstance class

문서의 특정 형식을 나타냅니다. 자신의 문서 유형을 추가하려면 이 클래스를 구현하십시오.

```csharp
public abstract class DocumentFormatInstance
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Password](../../groupdocs.redaction.integration/documentformatinstance/password) { get; set; } | 암호로 보호된 문서의 암호를 가져오거나 설정합니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| virtual [Initialize](../../groupdocs.redaction.integration/documentformatinstance/initialize)(DocumentFormatConfiguration, RedactorSettings) | 문서 형식 처리기의 인스턴스 초기화를 수행합니다. |
| [IsRedactionAccepted](../../groupdocs.redaction.integration/documentformatinstance/isredactionaccepted)(RedactionDescription) | 다음을 확인합니다.[`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) 구현하고 호출합니다(지정된 경우). |
| virtual [Load](../../groupdocs.redaction.integration/documentformatinstance/load)(Stream) | 스트림에서 문서를 로드합니다. |
| virtual [PerformBinaryCheck](../../groupdocs.redaction.integration/documentformatinstance/performbinarycheck)(Stream) | 지정된 스트림에 이 형식 인스턴스에서 지원하는 문서가 포함되어 있는지 확인합니다. |
| abstract [Save](../../groupdocs.redaction.integration/documentformatinstance/save)(Stream) | 문서를 스트림에 저장합니다. |

### 비고

**더 알아보기**

* 맞춤 형식 구현에 대한 자세한 내용: [사용자 지정 형식 처리기 만들기](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### 예

다음 예제는 사용자 지정 형식 처리기에 대한 빈 스텁을 만드는 방법을 보여줍니다.

다음 예제에서는 초기화 데이터를 사용하는 방법을 보여줍니다.

```csharp
public class DummyDocument : DocumentFormatInstance
{     
    public override void Load(Stream output)
    {
        // 파일 내용 로드
    }

    public override void Save(Stream output)
    {
        // 변경 사항을 파일에 저장합니다.
    }
}
```

```csharp
public class MyCustomHandler : DocumentFormatInstance
{
    private string MyProperty { get; set; }
    
    // 기타 사용자 지정 코드 
    ...

    public override void Initialize(DocumentFormatConfiguration config)
    {
        base.Initialize(config);
        if (config.InitializationData.ContainsKey("MyProperty"))
        {
            MyProperty = config.InitializationData["MyProperty"];
        }
    }
}

// 사용자 지정 형식을 GroupDocs.Redaction에 연결
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### 또한보십시오

* 네임스페이스 [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* 집회 [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->