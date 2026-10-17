---
title: "GroupDocs.Redaction for Python via .NET 설치"
linkTitle: "Installation"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "Windows, Linux 또는 macOS에서 GroupDocs.Redaction for Python via .NET을 설치합니다—PyPI 또는 사전 다운로드된 휠을 통해, Intel 및 Apple Silicon 빌드를 포함합니다."
type: docs
url: /ko/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction for Python via .NET은 [PyPI](https://pypi.org/project/groupdocs-redaction-net/)에 사전 빌드된 휠로 배포됩니다. PyPI 인덱스는 지원되는 각 플랫폼에 대해 별도의 휠을 호스팅하며, `pip`이 자동으로 올바른 휠을 선택합니다. 각 휠은 자체 포함형으로, 포함된 런타임과 모든 관리 종속성을 번들링하므로 Microsoft Office, OpenOffice, Adobe Acrobat 또는 별도의 런타임 설치가 필요하지 않습니다.

설치하기 전에 환경이 [System Requirements]() 항목에 나열된 지원 플랫폼 및 Python 버전과 일치하는지 확인하십시오.

## Install Package from PyPI

터미널을 열고 해당 플랫폼에 맞는 설치 명령을 실행하십시오:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

명령을 실행하면 다음과 유사한 출력이 표시됩니다:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

휠 파일 이름에는 운영 체제와 일치하는 플랫폼 접미사가 포함됩니다—예를 들어 Ubuntu/Debian에서는 `manylinux1_x86_64`, Apple Silicon에서는 `macosx_11_0_arm64`, 64비트 Windows에서는 `win_amd64`와 같습니다.

## Add the Package to `requirements.txt`

재현 가능한 환경을 위해, `requirements.txt`에 패키지 버전을 고정하십시오:

```txt
groupdocs-redaction-net==26.6.0
```

그런 다음 한 번에 모든 종속성을 설치하십시오:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

빌드 환경에서 PyPI에 접근할 수 없는 경우, [GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/)에서 적절한 휠을 다운로드하고 로컬에 설치하십시오. 휠은 다음 네 가지 플랫폼에 대해 제공됩니다:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

다운로드한 휠을 프로젝트 폴더에 넣은 다음, 설치하십시오:

```ps
py -m pip install ./groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl
```

```bash
python3 -m pip install ./groupdocs_redaction_net-26.6.0-py3-none-manylinux1_x86_64.whl
```

```bash
python3 -m pip install ./groupdocs_redaction_net-26.6.0-py3-none-macosx_10_14_x86_64.whl
```

```bash
python3 -m pip install ./groupdocs_redaction_net-26.6.0-py3-none-macosx_11_0_arm64.whl
```

예상 출력:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Windows에서는 추가 단계가 필요하지 않습니다. Linux 및 macOS에서는 렌더링 엔진이 의존하는 네이티브 라이브러리를 설치하십시오:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

버전 26.6.0에서는, **rasterization to PDF and image-area redaction run only on Windows** — Linux/macOS에서는 `System.PlatformNotSupportedException`을 발생시키며, 위의 네이티브 패키지는 해당 제한을 해제하지 않습니다. 텍스트, 메타데이터, 주석 및 페이지 레다션과 원본 형식 저장은 모든 플랫폼에서 작동합니다. 전체 기능 지원 매트릭스를 보려면 [System Requirements]()를 확인하십시오.

## Verify the Installation

패키지가 올바르게 가져와졌는지 확인하고 설치된 버전을 확인하십시오:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

버전과 위치를 확인하려면 `pip show groupdocs-redaction-net` 명령으로 설치된 패키지를 나열할 수도 있습니다.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
