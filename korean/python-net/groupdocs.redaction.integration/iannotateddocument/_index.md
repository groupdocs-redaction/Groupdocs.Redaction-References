---
title: "IAnnotatedDocument 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "주석(예: 댓글)에 접근하기 위해 필요한 메서드를 정의하며, 주석 삭제를 수행하기 위해 DocumentFormatInstance에서 파생된 클래스에서 구현되어야 합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.integration/iannotateddocument/
is_root: false
weight: 20
---


## IAnnotatedDocument class

주석(예: 코멘트)에 접근하기 위해 필요한 메서드를 정의하며, 주석 삭제를 수행하기 위해 [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-파생 클래스에서 구현되어야 합니다.

자세히 보기:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

IAnnotatedDocument 유형은 다음 멤버를 노출합니다:

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [delete_annotations](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/delete_annotations/#regular_expression) | 문서 내에서 정규식과 일치하는 모든 주석을 삭제합니다. |
| [delete_annotations_regex](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/delete_annotations_regex/) |  |
| [redact_annotation](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation/#regular_expression-replacement) | 문서 내 모든 주석에서 일치하는 텍스트를 교체합니다. |
| [redact_annotation_file](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation_file/) |  |
| [redact_annotation_regex](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation_regex/) |  |
| [redact_annotation_string](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation_string/) |  |

### 또 보기
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
