---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "LoadOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

LoadOptions 클래스의 새 인스턴스를 초기화합니다.

```python
def __init__(self):
    ...
```

## __init__ {#password}

지정된 비밀번호로 LoadOptions의 새 인스턴스를 초기화합니다.

```python
def __init__(self, password):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| password | `str` | 보호된 파일에 대한 비밀번호. |

### 예제

```python
    from groupdocs.redaction.options import LoadOptions

    # 비밀번호로 보호된 문서를 로드합니다.
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

지정된 pre‑rasterization 플래그로 새로운 LoadOptions 인스턴스를 초기화합니다.

```python
def __init__(self, pre_rasterize):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| pre_rasterize | `bool` | True이면 로드 시 래스터화를 강제합니다. |

## __init__ {#password-pre_rasterize}

지정된 비밀번호로 새로운 LoadOptions 인스턴스를 초기화합니다.

`pre_rasterize`가 True이면 문서를 로드할 때 래스터화가 강제됩니다.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| password | `str` | 보호된 파일에 대한 비밀번호. |
| pre_rasterize | `bool` | True이면 로드 시 래스터화를 강제합니다. |

### 예제

```python
from groupdocs.redaction.options import LoadOptions

# 비밀번호로 보호된 문서를 로드합니다.
load_opt = LoadOptions("mypassword")
```

### 또 보기
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
