---
title: RedactionResult
second_title: .NET API 참조용 GroupDocs.Redaction
description: 교정 작업의 결과를 나타냅니다.
type: docs
weight: 420
url: /ko/net/groupdocs.redaction/redactionresult/
---
## RedactionResult class

교정 작업의 결과를 나타냅니다.

```csharp
public class RedactionResult
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [ErrorMessage](../../groupdocs.redaction/redactionresult/errormessage) { get; } | 진단에 대한 오류 메시지를 가져옵니다. |
| [Status](../../groupdocs.redaction/redactionresult/status) { get; } | 실행 상태를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| static [Failed](../../groupdocs.redaction/redactionresult/failed)(string) | 실패 상태로 RedactionResult 클래스의 새 인스턴스를 초기화합니다. |
| static [Partial](../../groupdocs.redaction/redactionresult/partial)(string) | PartiallyApplied 상태로 RedactionResult 클래스의 새 인스턴스를 초기화합니다. |
| static [Skipped](../../groupdocs.redaction/redactionresult/skipped)(string) | 건너뛴 상태로 RedactionResult 클래스의 새 인스턴스를 초기화합니다. |
| static [Successful](../../groupdocs.redaction/redactionresult/successful)() | 적용(성공) 상태로 RedactionResult 클래스의 새 인스턴스를 초기화합니다. |

### 비고

**더 알아보기**

* 교정 결과에 대한 자세한 내용: [교정 기본 사항](https://docs.groupdocs.com/redaction/net/redaction-basics/)

### 또한보십시오

* 네임스페이스 [GroupDocs.Redaction](../../groupdocs.redaction)
* 집회 [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->