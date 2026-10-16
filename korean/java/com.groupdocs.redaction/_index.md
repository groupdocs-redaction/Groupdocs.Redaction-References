---
title: "com.groupdocs.redaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "이 패키지는 PDF 래스터 이미지 및 오피스 문서 형식의 문서에서 민감한 정보를 삭제하기 위한 클래스를 제공합니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.redaction/
---

이 패키지는 PDF, 래스터 이미지 및 오피스 문서 형식의 문서에서 민감한 정보를 삭제하는 클래스를 제공합니다.

이 패키지의 주요 클래스는 다음과 같습니다:

<br />

* [Redactor](../../com.groupdocs.redaction/redactor) is the entry point for redaction process.
* [Redaction](../../com.groupdocs.redaction/redaction) is abstract base class for all types of document redactions.
* [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) is pre-configured in XML set of redaction rules.
* [RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) provides information about redaction process results.

<br />




## 클래스

| 클래스 | 설명 |
| --- | --- |
| [DocumentInfo](../com.groupdocs.redaction/documentinfo) | 문서에 대한 정보를 나타냅니다. |
| [FileType](../com.groupdocs.redaction/filetype) | 파일 유형을 나타냅니다. |
| [PageInfo](../com.groupdocs.redaction/pageinfo) | 간략한 페이지 정보를 나타냅니다. |
| [Redaction](../com.groupdocs.redaction/redaction) | 모든 가림 처리 유형에 대한 기본 추상 클래스를 나타냅니다. |
| [RedactionPolicy](../com.groupdocs.redaction/redactionpolicy) | 적용할 특정 가림 처리 집합을 포함하는 정화 정책을 나타냅니다. |
| [RedactionResult](../com.groupdocs.redaction/redactionresult) | 가림 처리 작업의 결과를 나타냅니다. |
| [Redactor](../com.groupdocs.redaction/redactor) | 문서 가림 처리 프로세스를 제어하는 주요 클래스를 나타내며, 문서를 열고, 가림 처리하고, 저장할 수 있게 합니다. |
| [RedactorChangeLog](../com.groupdocs.redaction/redactorchangelog) | Redactor 클래스의 Apply() 메서드에 전달되는 가림 처리 목록에 대한 결과를 나타냅니다. |
| [RedactorLogEntry](../com.groupdocs.redaction/redactorlogentry) | 가림 처리 적용 결과를 나타냅니다. |

## 인터페이스

| 인터페이스 | 설명 |
| --- | --- |
| [IDocumentInfo](../com.groupdocs.redaction/idocumentinfo) | 기본 문서 정보를 가져오는 데 필요한 메서드를 정의합니다. |

## 열거형

| 열거형 | 설명 |
| --- | --- |
| [RedactionStatus](../com.groupdocs.redaction/redactionstatus) | 가림 처리 완료 상태를 나타냅니다. |
