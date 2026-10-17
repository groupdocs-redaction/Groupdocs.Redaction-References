---
title: "레다션 정책 사용"
linkTitle: "Use redaction policies"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "처리 방법을 알아보세요. 기업의 민감 데이터 제거 정책이 레다션 규칙 목록 형태라면, 코드에서 이를 지정할 필요가 없습니다. 사전 구성된 레다션 목록이 포함된 XML 문서를 지정할 수 있습니다."
type: docs
url: /ko/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


기업의 민감 데이터 제거 정책이 레다션 규칙 목록 형태라면, 코드에서 이를 지정할 필요가 없습니다. 사전 구성된 레다션 목록이 포함된 XML 문서를 지정할 수 있습니다.

아래는 레다션 정책 XML 파일의 예시입니다 (코드 속성 매핑은 명확합니다):

**RedactionPolicy.xml**

```xml
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns="http://www.groupdocs.com/redaction">  
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase="dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <eraseMetadataRedaction filter="All" />  
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
  <annotationRedaction regularExpression="(anno1)" replacement="foobar" />  
  <deleteAnnotationRedaction regularExpression="(anno2)" />  
  
  <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
  <imageAreaRedaction pointX="110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy> 
```
이 구조의 XML 문서를 만들기 위해 RedactionPolicy.save() 메서드를 사용할 수 있으며, 런타임에 레다션을 구성합니다.

다음 예제는 [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/)를 XML 파일로 저장하는 방법을 보여줍니다.
 

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    ReplacementOptions,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def create_redaction_policy():
    # 레다션 색상 정의
    color = Color.from_argb(255, 220, 20, 60)

    # 레다션 구성
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # 정책 생성
    policy = RedactionPolicy(redactions)

    # 레다션 정책을 XML 파일에 저장
    policy.save("./sample_policy.xml")
    print("Redactions policy saved to ./sample_policy.xml")

if __name__ == "__main__":
    create_redaction_policy()
```

  
```text
<?xml version="1.0"?>
<redactionPolicy>
  <exactPhraseRedaction actionType="ReplaceString" replacement="[Product]" searchPhrase="Redaction" />
  <regexRedaction actionType="DrawBox" color="#DC143C" regularExpression="\d{2}\s*\d{2}[^\d]*\d{6}" />
  <deleteAnnotationRedaction regularExpression="[.]*" />
  <eraseMetadataRedaction filter="All" />
</redactionPolicy>
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/create_redaction_policy/sample_policy.xml)

필요한 만큼 많은 정책을 보유할 수 있으며, 이를 로드하여 문서를 레다션할 수 있습니다.

아래 예제는 XML 파일에서 레다션 정책을 로드하고, 포함된 모든 규칙을 단일 `apply` 호출로 문서에 적용합니다:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # XML 파일에서 레다션 정책 로드
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # 문서를 로드하고 한 번의 호출로 전체 정책을 적용
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # 원본 형식을 유지하고 출력 이름에 접미사를 추가
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml`은 이 예제에서 사용된 정책 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml)를 클릭하십시오.

`sample.docx`은 이 예제에서 가린 문서입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) 를 클릭하십시오.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)
