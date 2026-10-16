---
title: "Redactor"
second_title: "GroupDocs.Redaction के लिए .NET API रेफ़रेंस"
description: "फ़ाइल पथ का उपयोग करके Redactorgroupdocs.redaction/redactor क्लास का नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

फ़ाइल पथ का उपयोग करके [`Redactor`](../../redactor) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public Redactor(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल का पथ |

### उदाहरण

निम्नलिखित उदाहरण दिखाता है कि कैसे रेडैक्शन के लिए दस्तावेज़ खोलें।

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // यहाँ हम रेडैक्शन करने के लिए दस्तावेज़ इंस्टेंस का उपयोग कर सकते हैं।
}
```

### साथ ही देखें

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

स्ट्रीम का उपयोग करके [`Redactor`](../../redactor) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public Redactor(Stream document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Stream | दस्तावेज़ की स्रोत स्ट्रीम |

### उदाहरण

निम्नलिखित उदाहरण दिखाता है कि कैसे स्ट्रीम से दस्तावेज़ खोलें।

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // यहाँ हम रेडैक्शन करने के लिए दस्तावेज़ इंस्टेंस का उपयोग कर सकते हैं।
    }
}
```

### साथ ही देखें

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

पासवर्ड-संरक्षित दस्तावेज़ के पथ का उपयोग करके [`Redactor`](../../redactor) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल का पथ। |
| loadOptions | LoadOptions | विकल्प, जिसमें पासवर्ड शामिल है। |

### साथ ही देखें

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

पासवर्ड-संरक्षित दस्तावेज़ के पथ और सेटिंग्स का उपयोग करके [`Redactor`](../../redactor) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल का पथ। |
| loadOptions | LoadOptions | फ़ाइल-निर्भर विकल्प, जिसमें पासवर्ड शामिल है। |
| सेटिंग्स | RedactorSettings | रेडैक्शन प्रक्रिया के लिए डिफ़ॉल्ट सेटिंग्स। |

### साथ ही देखें

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

पासवर्ड-संरक्षित दस्तावेज़ के लिए स्ट्रीम का उपयोग करके [`Redactor`](../../redactor) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Stream | स्रोत इनपुट स्ट्रीम। |
| loadOptions | LoadOptions | विकल्प, जिसमें पासवर्ड शामिल है। |

### उदाहरण

निम्न उदाहरण LoadOptions का उपयोग करके पासवर्ड-संरक्षित दस्तावेज़ों को खोलने का तरीका दर्शाता है।

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // यहाँ हम रेडैक्शन करने के लिए दस्तावेज़ इंस्टेंस का उपयोग कर सकते हैं।
}
```

### साथ ही देखें

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

स्ट्रीम और सेटिंग्स का उपयोग करके पासवर्ड-संरक्षित दस्तावेज़ के लिए [`Redactor`](../../redactor) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Stream | स्रोत इनपुट स्ट्रीम। |
| loadOptions | LoadOptions | विकल्प, जिसमें पासवर्ड शामिल है। |
| सेटिंग्स | RedactorSettings | रेडैक्शन प्रक्रिया के लिए डिफ़ॉल्ट सेटिंग्स। |

### उदाहरण

निम्न उदाहरण LoadOptions का उपयोग करके पासवर्ड-संरक्षित दस्तावेज़ों को खोलने का तरीका दर्शाता है।

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // यहाँ हम रेडैक्शन करने के लिए दस्तावेज़ इंस्टेंस का उपयोग कर सकते हैं।
}
```

### साथ ही देखें

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
