---
title: "GroupDocs.Redaction for Python via .NET स्थापित करें"
linkTitle: "Installation"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "Windows, Linux, या macOS पर GroupDocs.Redaction for Python via .NET स्थापित करें — PyPI से या प्री-डाउनलोडेड व्हील से, जिसमें Intel और Apple Silicon बिल्ड शामिल हैं।"
type: docs
url: /hi/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction for Python via .NET को एक प्री-बिल्ट व्हील के रूप में [PyPI](https://pypi.org/project/groupdocs-redaction-net/) पर वितरित किया जाता है। PyPI इंडेक्स प्रत्येक समर्थित प्लेटफ़ॉर्म के लिए एक अलग व्हील रखता है, और `pip` स्वचालित रूप से सही वाला चुन लेता है। प्रत्येक व्हील स्व-निहित है: यह एम्बेडेड रनटाइम और सभी प्रबंधित निर्भरताओं को बंडल करता है, इसलिए Microsoft Office, OpenOffice, Adobe Acrobat, या अलग रनटाइम इंस्टॉल की आवश्यकता नहीं होती।

इंस्टॉल करने से पहले, सुनिश्चित करें कि आपका पर्यावरण समर्थित प्लेटफ़ॉर्म और Python संस्करणों से मेल खाता है, जैसा कि [System Requirements]() विषय में सूचीबद्ध है।

## Install Package from PyPI

एक टर्मिनल खोलें और अपने प्लेटफ़ॉर्म के लिए इंस्टॉल कमांड चलाएँ:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

कमांड चलाने के बाद आपको इस तरह का आउटपुट दिखना चाहिए:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

व्हील फ़ाइल का नाम एक प्लेटफ़ॉर्म उपसर्ग शामिल करेगा जो आपके ऑपरेटिंग सिस्टम से मेल खाता है — उदाहरण के लिए Ubuntu/Debian पर `manylinux1_x86_64`, Apple Silicon पर `macosx_11_0_arm64`, या 64-बिट Windows पर `win_amd64`।

## Add the Package to `requirements.txt`

पुनरुत्पादक वातावरण के लिए, अपने `requirements.txt` में पैकेज संस्करण को पिन करें:

```txt
groupdocs-redaction-net==26.6.0
```

फिर सभी निर्भरताओं को एक ही चरण में इंस्टॉल करें:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

यदि आपका बिल्ड वातावरण PyPI तक नहीं पहुँच सकता, तो उपयुक्त व्हील को [GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/) से डाउनलोड करें और स्थानीय रूप से इंस्टॉल करें। व्हील निम्नलिखित चार प्लेटफ़ॉर्म के लिए प्रकाशित किए गए हैं:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

डाउनलोड किया गया व्हील अपने प्रोजेक्ट फ़ोल्डर में रखें, फिर इसे इंस्टॉल करें:

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

अपेक्षित आउटपुट:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Windows पर कोई अतिरिक्त कदम आवश्यक नहीं हैं। Linux और macOS पर, रेंडरिंग इंजन की निर्भरता वाली नेटिव लाइब्रेरीज़ इंस्टॉल करें:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

संस्करण 26.6.0 में, **rasterization to PDF and image-area redaction run only on Windows** — Linux/macOS पर यह `System.PlatformNotSupportedException` उठाते हैं, और ऊपर के नेटिव पैकेज इस प्रतिबंध को नहीं हटाते। टेक्स्ट, मेटाडेटा, एनोटेशन, और पेज रिडैक्शन तथा मूल-फ़ॉर्मेट सेव्स हर प्लेटफ़ॉर्म पर काम करते हैं। पूर्ण फीचर‑सपोर्ट मैट्रिक्स के लिए देखें [System Requirements]().

## Verify the Installation

पैकेज को सही तरीके से इम्पोर्ट हुआ है यह पुष्टि करें और स्थापित संस्करण जाँचें:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

आप `pip show groupdocs-redaction-net` के साथ स्थापित पैकेज की सूची भी देख सकते हैं ताकि संस्करण और स्थान की पुष्टि हो सके।

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
