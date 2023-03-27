---
title: AddAdvancedOption
second_title: .NET API संदर्भ के लिए GroupDocs.Redaction
description: आप लगू करने के लए एक उन्नत रेखंकन वकल्प क पंजकृत करने के लए इस वध क उपयग कर सकते हैं
type: docs
weight: 70
url: /hi/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

आप लागू करने के लिए एक उन्नत रेखांकन विकल्प को पंजीकृत करने के लिए इस विधि का उपयोग कर सकते हैं।

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | चयनित प्रभाव प्रकार (ग्रेस्केल, बॉर्डर, आदि) के बारे में जानकारी प्रदान करता है। |

### उदाहरण

निम्न उदाहरण प्रदर्शित करता है कि डिफ़ॉल्ट सेटिंग्स के साथ उन्नत रेखांकन विकल्पों को कैसे लागू किया जाए।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // दस्तावेज़ को डिफ़ॉल्ट विकल्पों के साथ सहेजें (पृष्ठों को छवियों में बदलें, पीडीएफ के रूप में सहेजें)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

### यह सभी देखें

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* नाम स्थान [GroupDocs.Redaction.Options](../../rasterizationoptions)
* सभा [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

आप लागू करने के लिए एक उन्नत रेखांकन विकल्प को पंजीकृत करने के लिए इस विधि का उपयोग कर सकते हैं।

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | चयनित प्रभाव प्रकार (ग्रेस्केल, बॉर्डर, आदि) के बारे में जानकारी प्रदान करता है। |
| parameters | Dictionary`2 | दिए गए प्रभाव के लिए पैरामीटर, जैसे घूर्णन कोण |

### उदाहरण

निम्न उदाहरण प्रदर्शित करता है कि डिफ़ॉल्ट सेटिंग्स के साथ उन्नत रेखांकन विकल्पों को कैसे लागू किया जाए।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // दस्तावेज़ को डिफ़ॉल्ट विकल्पों के साथ सहेजें (पृष्ठों को छवियों में बदलें, पीडीएफ के रूप में सहेजें)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

निम्न उदाहरण दर्शाता है कि कस्टम सेटिंग्स के साथ बॉर्डर उन्नत रेखांकन विकल्प को कैसे लागू किया जाए।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // दस्तावेज़ को कस्टम बॉर्डर के साथ सहेजें
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

निम्नलिखित उदाहरण दर्शाता है कि कस्टम सेटिंग्स के साथ नॉइज़ एडवांस्ड रैस्टराइज़ेशन विकल्प को कैसे लागू किया जाए।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // दस्तावेज़ को कस्टम संख्या और शोर प्रभावों के आकार के साथ सहेजें
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

निम्न उदाहरण प्रदर्शित करता है कि कस्टम सेटिंग्स के साथ टिल्ट एडवांस्ड रैस्टराइज़ेशन विकल्प को कैसे लागू किया जाए।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // दस्तावेज़ को कस्टम झुकाव प्रभाव से सहेजें
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### यह सभी देखें

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* नाम स्थान [GroupDocs.Redaction.Options](../../rasterizationoptions)
* सभा [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
