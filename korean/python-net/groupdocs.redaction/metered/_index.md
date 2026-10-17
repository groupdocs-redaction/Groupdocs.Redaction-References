---
title: "Metered 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "사용량 기반(종량제) 라이선스를 관리합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/metered/
is_root: false
weight: 80
---


## Metered class

사용량 기반(종량제) 라이선스를 관리합니다.

Metered 라이선스는 실제 사용량(보통 페이지 또는
처리된 문서) 기준으로 청구됩니다. 공개/비공개 키 쌍을 한 번 설정합니다.
애플리케이션 시작 시; 래퍼가 사용량을 GroupDocs에 보고합니다.
백그라운드에서 라이선스 서버에 전송합니다.

Metered 타입은 다음 멤버를 노출합니다:

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [get_consumption_credit](/redaction/python-net/groupdocs.redaction/metered/get_consumption_credit/) | 현재 키에 대한 남은 측정 크레딧을 반환합니다. |
| [get_consumption_quantity](/redaction/python-net/groupdocs.redaction/metered/get_consumption_quantity/) | 지금까지 사용된 총 측정 수량을 반환합니다. |
| [set_metered_key](/redaction/python-net/groupdocs.redaction/metered/set_metered_key/#public_key-private_key) | 주어진 공개/비공개 키 쌍으로 측정 청구를 활성화합니다. |

### 또 보기
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
