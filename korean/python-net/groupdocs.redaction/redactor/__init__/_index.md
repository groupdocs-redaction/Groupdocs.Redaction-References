---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "파일 경로를 사용하여 새로운 Redactor 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

파일 경로를 사용하여 새로운 Redactor 인스턴스를 초기화합니다.

```python
def __init__(self, file_path):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| file_path | `str` | 파일 경로. |

### 예제

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # 여기서 redaction 작업을 수행합니다
    pass
```

## __init__ {#document}

스트림을 사용하여 새로운 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 인스턴스를 초기화합니다.

```python
def __init__(self, document):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| document | `io.RawIOBase` | 문서의 소스 스트림. |

### 예제

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # 문서를 바이너리 스트림으로 열기
    with open("./sample.pdf", "rb") as stream:
        # 스트림에서 문서 로드
        with Redactor(stream) as redactor:
            # 여기서 redaction을 수행합니다
            pass
```

## __init__ {#file_path-load_options}

경로를 사용하여 비밀번호로 보호된 문서에 대한 새로운 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 인스턴스를 초기화합니다.

```python
def __init__(self, file_path, load_options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| file_path | `str` | 파일 경로. |
| load_options | `LoadOptions` | 옵션, 비밀번호 포함. |

### 예제

```python
from groupdocs.redaction import Redactor

# 파일 경로에서 비밀번호로 보호된 문서를 로드합니다
with Redactor("protected.docx") as redactor:
    # 여기서 redaction 작업을 수행합니다
    pass
```

## __init__ {#file_path-load_options-settings}

경로와 설정을 사용하여 비밀번호로 보호된 문서에 대한 새로운 Redactor 인스턴스를 초기화합니다.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| file_path | `str` | 파일 경로. |
| load_options | `LoadOptions` | 파일에 따라 달라지는 옵션, 비밀번호 포함. |
| settings | `RedactorSettings` | redaction 프로세스의 기본 설정. |

### 예제

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

스트림을 사용하여 비밀번호로 보호된 문서에 대한 새로운 Redactor 인스턴스를 초기화합니다.

```python
def __init__(self, document, load_options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| document | `io.RawIOBase` | 소스 입력 스트림. |
| load_options | `LoadOptions` | 옵션, 비밀번호 포함. |

### 예제

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # 보호된 PDF를 바이너리 스트림으로 엽니다
    with open(r"C:\sample.pdf", "rb") as stream:
        # `LoadOptions`를 통해 비밀번호를 제공합니다
        load_options = LoadOptions("mypassword")
        # 스트림과 로드 옵션으로 Redactor를 초기화합니다
        with Redactor(stream, load_options) as redactor:
            # 여기서 redaction 작업을 수행합니다
            pass
```

## __init__ {#document-load_options-settings}

스트림과 설정을 사용하여 비밀번호로 보호된 문서에 대한 새로운 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 인스턴스를 초기화합니다.

```python
def __init__(self, document, load_options, settings):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| document | `io.RawIOBase` | 소스 입력 스트림. |
| load_options | `LoadOptions` | 옵션, 비밀번호 포함. |
| settings | `RedactorSettings` | 편집 프로세스에 대한 기본 설정. |

### 또 보기
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
