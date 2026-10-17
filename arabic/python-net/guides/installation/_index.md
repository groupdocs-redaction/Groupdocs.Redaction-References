---
title: "ثبّت GroupDocs.Redaction for Python via .NET"
linkTitle: "Installation"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ثبّت GroupDocs.Redaction for Python via .NET على Windows أو Linux أو macOS — من PyPI أو من عجلة تم تنزيلها مسبقًا، بما في ذلك إصدارات Intel وApple Silicon."
type: docs
url: /ar/python-net/guides/installation/
is_root: false
weight: 10
---


يتم توزيع GroupDocs.Redaction للبايثون عبر .NET كحزمة wheel مُعدة مسبقًا على [PyPI](https://pypi.org/project/groupdocs-redaction-net/). يستضيف فهرس PyPI حزمة wheel منفصلة لكل منصة مدعومة، ويختار `pip` الحزمة الصحيحة تلقائيًا. كل wheel مكتملة ذاتيًا: فهي تضم وقت التشغيل المدمج وكل الاعتماديات المُدارة، لذا لا يلزم تثبيت Microsoft Office أو OpenOffice أو Adobe Acrobat أو وقت تشغيل منفصل.

قبل التثبيت، تأكد من أن بيئتك تتطابق مع المنصات المدعومة وإصدارات بايثون المذكورة في موضوع [System Requirements]().

## Install Package from PyPI

افتح طرفية ونفّذ أمر التثبيت المناسب لمنصتك:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

بعد تشغيل الأمر يجب أن ترى مخرجات مشابهة لـ:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

سيتضمن اسم ملف الـ wheel لاحقة منصة تتطابق مع نظام التشغيل الخاص بك — على سبيل المثال `manylinux1_x86_64` على Ubuntu/Debian، `macosx_11_0_arm64` على Apple Silicon، أو `win_amd64` على Windows 64‑bit.

## Add the Package to `requirements.txt`

لضمان بيئات قابلة لإعادة الإنتاج، قم بتثبيت نسخة الحزمة في ملف `requirements.txt` الخاص بك:

```txt
groupdocs-redaction-net==26.6.0
```

ثم قم بتثبيت جميع الاعتماديات في خطوة واحدة:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

إذا كان بيئة البناء الخاصة بك لا تستطيع الوصول إلى PyPI، قم بتنزيل الـ wheel المناسب من [موقع إصدارات GroupDocs](https://releases.groupdocs.com/redaction/python-net/) وقم بتثبيته محليًا. تُنشر الـ wheels للمنصات الأربعة التالية:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

ضع الـ wheel الذي تم تنزيله في مجلد مشروعك، ثم قم بتثبيته:

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

المخرجات المتوقعة:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

على Windows لا توجد خطوات إضافية مطلوبة. على Linux و macOS، قم بتثبيت المكتبات الأصلية التي يعتمد عليها محرك العرض:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

في الإصدار 26.6.0، **التصوير إلى PDF وإزالة التغطية عن مناطق الصور يعمل فقط على Windows** — على Linux/macOS يتم رفع استثناء `System.PlatformNotSupportedException`، ولا تُزيل الحزم الأصلية المذكورة أعلاه هذا القيد. النص، والبيانات الوصفية، والتعليقات التوضيحية، وإزالة تغطية الصفحات وحفظ الصيغ الأصلية تعمل على جميع المنصات. راجع [System Requirements]() للحصول على مصفوفة الدعم الكاملة للميزات.

## Verify the Installation

تأكد من استيراد الحزمة بشكل صحيح وتحقق من النسخة المثبتة:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

يمكنك أيضًا سرد الحزمة المثبتة باستخدام `pip show groupdocs-redaction-net` لتأكيد النسخة والموقع.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
