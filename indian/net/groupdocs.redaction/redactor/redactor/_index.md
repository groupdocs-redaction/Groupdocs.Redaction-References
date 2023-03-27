---
title: Redactor
second_title: .NET API संदर्भ के लिए GroupDocs.Redaction
description: क एक नय उदहरण शुरू करत हैRedactorgroupdocs.redaction/redactor वर्ग फ़इल पथ. क उपयग कर
type: docs
weight: 10
url: /hi/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

का एक नया उदाहरण शुरू करता है[`Redactor`](../../redactor) वर्ग फ़ाइल पथ. का उपयोग कर

```csharp
public Redactor(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल का पथ |

### उदाहरण

निम्न उदाहरण प्रदर्शित करता है कि संपादन के लिए दस्तावेज़ कैसे खोला जाए।

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // यहां हम रिडक्शन करने के लिए डॉक्यूमेंट इंस्टेंस का उपयोग कर सकते हैं
}
```

### यह सभी देखें

* class [Redactor](../../redactor)
* नाम स्थान [GroupDocs.Redaction](../../redactor)
* सभा [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

का एक नया उदाहरण शुरू करता है[`Redactor`](../../redactor) धारा का उपयोग कर कक्षा।

```csharp
public Redactor(Stream document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| document | Stream | दस्तावेज़ की स्रोत धारा |

### उदाहरण

निम्न उदाहरण प्रदर्शित करता है कि स्ट्रीम से दस्तावेज़ कैसे खोलें।

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // यहां हम रिडक्शन करने के लिए डॉक्यूमेंट इंस्टेंस का उपयोग कर सकते हैं
    }
}
```

### यह सभी देखें

* class [Redactor](../../redactor)
* नाम स्थान [GroupDocs.Redaction](../../redactor)
* सभा [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

का एक नया उदाहरण शुरू करता है[`Redactor`](../../redactor) अपने पथ का उपयोग करते हुए पासवर्ड-सुरक्षित दस्तावेज़ के लिए क्लास .

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फाइल करने के लिए पथ। |
| loadOptions | LoadOptions | पासवर्ड सहित विकल्प। |

### यह सभी देखें

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* नाम स्थान [GroupDocs.Redaction](../../redactor)
* सभा [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

का एक नया उदाहरण शुरू करता है[`Redactor`](../../redactor) अपने पथ और सेटिंग्स का उपयोग करके पासवर्ड-सुरक्षित दस्तावेज़ के लिए वर्ग।

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फाइल करने के लिए पथ। |
| loadOptions | LoadOptions | पासवर्ड सहित फ़ाइल-निर्भर विकल्प। |
| settings | RedactorSettings | सुधार प्रक्रिया के लिए डिफ़ॉल्ट सेटिंग्स। |

### यह सभी देखें

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* नाम स्थान [GroupDocs.Redaction](../../redactor)
* सभा [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

का एक नया उदाहरण शुरू करता है[`Redactor`](../../redactor) स्ट्रीम. का उपयोग करके पासवर्ड से सुरक्षित दस्तावेज़ के लिए वर्ग

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| document | Stream | स्रोत इनपुट स्ट्रीम। |
| loadOptions | LoadOptions | पासवर्ड सहित विकल्प। |

### उदाहरण

निम्न उदाहरण दर्शाता है कि LoadOptions का उपयोग करके पासवर्ड-सुरक्षित दस्तावेज़ कैसे खोलें।

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // यहां हम रिडक्शन करने के लिए डॉक्यूमेंट इंस्टेंस का उपयोग कर सकते हैं
}
```

### यह सभी देखें

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* नाम स्थान [GroupDocs.Redaction](../../redactor)
* सभा [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

का एक नया उदाहरण शुरू करता है[`Redactor`](../../redactor)स्ट्रीम और सेटिंग का उपयोग करके पासवर्ड से सुरक्षित दस्तावेज़ के लिए क्लास.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| document | Stream | स्रोत इनपुट स्ट्रीम। |
| loadOptions | LoadOptions | पासवर्ड सहित विकल्प। |
| settings | RedactorSettings | सुधार प्रक्रिया के लिए डिफ़ॉल्ट सेटिंग्स। |

### उदाहरण

निम्न उदाहरण दर्शाता है कि LoadOptions का उपयोग करके पासवर्ड-सुरक्षित दस्तावेज़ कैसे खोलें।

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // यहां हम रिडक्शन करने के लिए डॉक्यूमेंट इंस्टेंस का उपयोग कर सकते हैं
}
```

### यह सभी देखें

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* नाम स्थान [GroupDocs.Redaction](../../redactor)
* सभा [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
