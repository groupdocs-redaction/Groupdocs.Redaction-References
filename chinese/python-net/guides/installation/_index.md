---
title: "安装 GroupDocs.Redaction for Python via .NET"
linkTitle: "Installation"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "在 Windows、Linux 或 macOS 上安装 GroupDocs.Redaction for Python via .NET——可通过 PyPI 或预下载的 wheel，包含 Intel 和 Apple Silicon 构建。"
type: docs
url: /zh/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction for Python via .NET 以预构建的 wheel 形式分发在 [PyPI](https://pypi.org/project/groupdocs-redaction-net/)。PyPI 索引为每个受支持平台提供单独的 wheel，`pip` 会自动选择正确的版本。每个 wheel 都是自包含的：它捆绑嵌入的运行时和所有托管依赖项，无需安装 Microsoft Office、OpenOffice、Adobe Acrobat 或其他运行时。

安装前，请确认您的环境符合 [System Requirements]() 章节中列出的受支持平台和 Python 版本。

## Install Package from PyPI

打开终端并为您的平台运行安装命令：

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

运行命令后，您应该会看到类似以下的输出：

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

wheel 文件名将包含与操作系统匹配的平台后缀，例如在 Ubuntu/Debian 上为 `manylinux1_x86_64`，在 Apple Silicon 上为 `macosx_11_0_arm64`，或在 64 位 Windows 上为 `win_amd64`。

## Add the Package to `requirements.txt`

为了可复现的环境，请在你的 `requirements.txt` 中固定包的版本：

```txt
groupdocs-redaction-net==26.6.0
```

然后一次性安装所有依赖：

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

如果你的构建环境无法访问 PyPI，请从 [GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/) 下载相应的 wheel 并在本地安装。Wheel 已为以下四个平台发布：

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

将下载的 wheel 放入项目文件夹，然后进行安装：

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

预期输出：

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

在 Windows 上无需额外步骤。 在 Linux 和 macOS 上，需要安装渲染引擎依赖的本机库：

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

在 26.6.0 版本中，**rasterization to PDF and image-area redaction run only on Windows** — 在 Linux/macOS 上会抛出 `System.PlatformNotSupportedException`，且上述本机包并未解除此限制。文本、元数据、注释以及页面遮蔽和原始格式保存在所有平台均可工作。请参阅 [System Requirements]() 了解完整的功能支持矩阵。

## Verify the Installation

确认包已正确导入并检查已安装的版本：

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

你也可以使用 `pip show groupdocs-redaction-net` 列出已安装的包，以确认版本和位置。

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
