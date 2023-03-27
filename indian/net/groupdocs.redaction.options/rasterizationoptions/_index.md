---
title: RasterizationOptions
second_title: .NET API संदर्भ के लिए GroupDocs.Redaction
description: फइलं क पडएफ में बदलने के लए वकल्प प्रदन करत है
type: docs
weight: 350
url: /hi/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

फाइलों को पीडीएफ में बदलने के लिए विकल्प प्रदान करता है।

```csharp
public class RasterizationOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | एक नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | पीडीएफ अनुपालन स्तर प्राप्त या सेट करता है। |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | एक मान प्राप्त या सेट करता है जो दर्शाता है कि दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित करने और एक पीडीएफ फाइल में डालने की आवश्यकता है या नहीं। रेखांकन से बचने के लिए डिफ़ॉल्ट रूप से TRUE, FALSE पर सेट करें। |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | एक संकेतक प्राप्त करता है, जो उन्नत रेखांकन विकल्प सेट होने पर सत्य है। |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | PDF में कनवर्ट किए जाने वाले पृष्ठों की संख्या प्राप्त करता है या सेट करता है. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | PDF में कनवर्ट करने के लिए पहले पृष्ठ (0-आधारित) की अनुक्रमणिका प्राप्त या सेट करता है. |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | आप लागू करने के लिए एक उन्नत रेखांकन विकल्प को पंजीकृत करने के लिए इस विधि का उपयोग कर सकते हैं। |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | आप लागू करने के लिए एक उन्नत रेखांकन विकल्प को पंजीकृत करने के लिए इस विधि का उपयोग कर सकते हैं। |

### टिप्पणियों

**और अधिक जानें**

* दस्तावेज़ को रास्टराइज़ किए गए PDF के रूप में सहेजने के बारे में अधिक विवरण: [रास्टराइज्ड पीडीएफ में सेव करें](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* रेखांकन विकल्पों के बारे में अधिक विवरण: [रास्‍टरीकृत PDF के लिए विशिष्‍ट पृष्‍ठों का चयन करें](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### उदाहरण

निम्न उदाहरण दर्शाता है कि रास्टराइजेशन प्रक्रिया के लिए विकल्प कैसे सेट करें।

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // पहली स्लाइड पर संवेदनशील डेटा को रिडक्ट करें 
    
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

* नाम स्थान [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* सभा [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
