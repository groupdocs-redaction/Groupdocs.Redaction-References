---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction के लिए .NET API रेफ़रेंस"
description: "फ़ाइलों को PDF में परिवर्तित करने के विकल्प प्रदान करता है।"
type: docs
weight: 420
url: /hi/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

फ़ाइलों को PDF में परिवर्तित करने के विकल्प प्रदान करता है।

```csharp
public class RasterizationOptions
```

## Constructors

| नाम | विवरण |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | एक नया इंस्टेंस प्रारंभ करता है। |

## Properties

| नाम | विवरण |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | PDF अनुपालन स्तर को प्राप्त करता है या सेट करता है। |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि क्या दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करके एकल PDF फ़ाइल में रखा जाना चाहिए। डिफ़ॉल्ट रूप से TRUE, रास्टराइज़ेशन से बचने के लिए FALSE सेट करें। |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | एक संकेतक प्राप्त करता है, जो तब सत्य होता है जब उन्नत रास्टराइज़ेशन विकल्प सेट किए गए हों। |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | PDF में परिवर्तित किए जाने वाले पृष्ठों की संख्या को प्राप्त करता है या सेट करता है। |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | PDF में परिवर्तित करने के लिए पहले पृष्ठ (0-आधारित) का सूचकांक प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | आप इस मेथड का उपयोग करके लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत कर सकते हैं। |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | आप इस मेथड का उपयोग करके लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत कर सकते हैं। |

### टिप्पणियाँ

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### उदाहरण

निम्नलिखित उदाहरण रास्टराइज़ेशन प्रक्रिया के लिए विकल्प सेट करने का तरीका दर्शाता है।

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // पहली स्लाइड पर संवेदनशील डेटा को रेडैक्ट करें
    
        var rasterizationOptions = new RasterizationOptions();
        rasterizationOptions.PageIndex = 0;
        rasterizationOptions.PageCount = 1;
        rasterizationOptions.Compliance = PdfComplianceLevel.PdfA1a;
        using (var stream = File.Open(Path.Combine(@"C:\Temp", "PresentationFirstSlide.pdf")))
        {
            redactor.Save(stream, rasterizationOptions);
        }
    }      
```

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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
