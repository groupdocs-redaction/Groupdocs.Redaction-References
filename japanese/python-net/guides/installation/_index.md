---
title: "GroupDocs.Redaction for Python via .NET をインストールする"
linkTitle: "Installation"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "GroupDocs.Redaction for Python via .NET を Windows、Linux、macOS にインストールします — PyPI または事前にダウンロードした wheel から、Intel と Apple Silicon ビルドを含めてインストールできます。"
type: docs
url: /ja/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction for Python via .NET は [PyPI](https://pypi.org/project/groupdocs-redaction-net/) で配布されている事前構築の wheel です。PyPI インデックスはサポートされている各プラットフォーム用に個別の wheel をホストしており、`pip` が自動的に適切なものを選択します。各 wheel は自己完結型で、組み込みランタイムとすべての管理依存関係をバンドルしているため、Microsoft Office、OpenOffice、Adobe Acrobat、または別個のランタイムのインストールは不要です。

インストール前に、環境が [System Requirements]() トピックに記載されたサポートプラットフォームと Python バージョンに合致していることを確認してください。

## Install Package from PyPI

ターミナルを開き、使用するプラットフォームに合わせてインストールコマンドを実行してください:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

コマンドを実行すると、以下のような出力が表示されます:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

wheel ファイル名には、使用しているオペレーティングシステムに一致するプラットフォームサフィックスが含まれます。例として Ubuntu/Debian の `manylinux1_x86_64`、Apple Silicon の `macosx_11_0_arm64`、64 ビット Windows の `win_amd64` などがあります。

## Add the Package to `requirements.txt`

再現可能な環境のために、`requirements.txt` にパッケージのバージョンを固定してください：

```txt
groupdocs-redaction-net==26.6.0
```

次に、すべての依存関係を一括でインストールしてください：

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

ビルド環境が PyPI にアクセスできない場合は、[GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/) から適切なホイールをダウンロードし、ローカルにインストールしてください。ホイールは以下の 4 つのプラットフォーム向けに公開されています：

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

ダウンロードしたホイールをプロジェクトフォルダーに配置し、次にインストールしてください：

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

期待される出力：

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Windows では追加の手順は不要です。Linux および macOS では、レンダリングエンジンが依存するネイティブライブラリをインストールしてください：

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

バージョン 26.6.0 では、**rasterization to PDF and image-area redaction run only on Windows** — Linux/macOS では `System.PlatformNotSupportedException` が発生し、上記のネイティブパッケージではその制限が解除されません。テキスト、メタデータ、注釈、ページの赤字および元の形式での保存はすべてのプラットフォームで機能します。完全な機能サポートマトリックスについては、[System Requirements]() を参照してください。

## Verify the Installation

パッケージが正しくインポートされたことを確認し、インストールされたバージョンをチェックしてください：

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

`pip show groupdocs-redaction-net` を使用してインストールされたパッケージを一覧表示し、バージョンと場所を確認することもできます。

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
