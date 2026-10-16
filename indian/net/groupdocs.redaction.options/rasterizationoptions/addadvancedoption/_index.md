---
title: "AddAdvancedOption"
second_title: "GroupDocs.Redaction के लिए .NET API रेफ़रेंस"
description: "आप इस मेथड का उपयोग करके लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत कर सकते हैं।"
type: docs
weight: 70
url: /hi/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

आप इस मेथड का उपयोग करके लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत कर सकते हैं।

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | चयनित प्रभाव प्रकार (ग्रेस्केल, बॉर्डर, आदि) के बारे में जानकारी प्रदान करता है। |

### उदाहरण

निम्न उदाहरण दिखाता है कि डिफ़ॉल्ट सेटिंग्स के साथ उन्नत रास्टराइज़ेशन विकल्पों को कैसे लागू करें।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // डिफ़ॉल्ट विकल्पों के साथ दस्तावेज़ सहेजें (पृष्ठों को छवियों में बदलें, PDF के रूप में सहेजें)
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

### साथ ही देखें

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

आप इस मेथड का उपयोग करके लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत कर सकते हैं।

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | चयनित प्रभाव प्रकार (ग्रेस्केल, बॉर्डर, आदि) के बारे में जानकारी प्रदान करता है। |
| parameters | Dictionary`2 | दिए गए प्रभाव के पैरामीटर, जैसे घूर्णन कोण |

### उदाहरण

निम्न उदाहरण दिखाता है कि डिफ़ॉल्ट सेटिंग्स के साथ उन्नत रास्टराइज़ेशन विकल्पों को कैसे लागू करें।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // डिफ़ॉल्ट विकल्पों के साथ दस्तावेज़ सहेजें (पृष्ठों को छवियों में बदलें, PDF के रूप में सहेजें)
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

निम्न उदाहरण दिखाता है कि कस्टम सेटिंग्स के साथ बॉर्डर उन्नत रास्टराइज़ेशन विकल्प को कैसे लागू करें।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // कस्टम बॉर्डर के साथ दस्तावेज़ सहेजें
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

निम्न उदाहरण दिखाता है कि कस्टम सेटिंग्स के साथ शोर उन्नत रास्टराइज़ेशन विकल्प को कैसे लागू करें।

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

निम्नलिखित उदाहरण दिखाता है कि कैसे कस्टम सेटिंग्स के साथ टिल्ट उन्नत रास्टराइज़ेशन विकल्प लागू किया जाए।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // कस्टम टिल्ट प्रभाव के साथ दस्तावेज़ सहेजें
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### साथ ही देखें

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
