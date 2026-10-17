---
title: "Instalar GroupDocs.Redaction para Python vía .NET"
linkTitle: "Installation"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Instalar GroupDocs.Redaction para Python vía .NET en Windows, Linux o macOS — desde PyPI o desde una rueda predescargada, incluidas versiones para Intel y Apple Silicon."
type: docs
url: /es/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction para Python a través de .NET se distribuye como una rueda preconstruida en [PyPI](https://pypi.org/project/groupdocs-redaction-net/). El índice de PyPI aloja una rueda separada para cada plataforma compatible, y `pip` selecciona la correcta automáticamente. Cada rueda es autónoma: incluye el tiempo de ejecución incrustado y todas las dependencias gestionadas, por lo que no se requiere instalar Microsoft Office, OpenOffice, Adobe Acrobat ni un tiempo de ejecución separado.

Antes de instalar, confirme que su entorno coincide con las plataformas compatibles y las versiones de Python enumeradas en el tema [Requisitos del sistema]().

## Install Package from PyPI

Abra una terminal y ejecute el comando de instalación para su plataforma:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

Después de ejecutar el comando debería ver una salida similar a:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

El nombre del archivo de la rueda incluirá un sufijo de plataforma que coincida con su sistema operativo — por ejemplo `manylinux1_x86_64` en Ubuntu/Debian, `macosx_11_0_arm64` en Apple Silicon, o `win_amd64` en Windows de 64 bits.

## Add the Package to `requirements.txt`

Para entornos reproducibles, fije la versión del paquete en su `requirements.txt`:

```txt
groupdocs-redaction-net==26.6.0
```

Luego instale todas las dependencias en un solo paso:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Si su entorno de compilación no puede acceder a PyPI, descargue la rueda adecuada desde el [sitio web de GroupDocs Releases](https://releases.groupdocs.com/redaction/python-net/) e instálela localmente. Las ruedas se publican para las siguientes cuatro plataformas:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

Coloque la rueda descargada en la carpeta de su proyecto y luego instálela:

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

Salida esperada:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

En Windows no se requieren pasos adicionales. En Linux y macOS, instale las bibliotecas nativas de las que depende el motor de renderizado:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

En la versión 26.6.0, **rasterization to PDF and image-area redaction run only on Windows** — en Linux/macOS generan `System.PlatformNotSupportedException`, y los paquetes nativos anteriores no eliminan esa restricción. La redacción de texto, metadatos, anotaciones y páginas y los guardados en formato original funcionan en todas las plataformas. Consulte [Requisitos del sistema]() para la matriz completa de compatibilidad de funciones.

## Verify the Installation

Confirme que el paquete se importó correctamente y verifique la versión instalada:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

También puede listar el paquete instalado con `pip show groupdocs-redaction-net` para confirmar la versión y la ubicación.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
