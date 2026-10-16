---
title: "Redactor"
second_title: "GroupDocs.Redaction के लिए .NET API रेफ़रेंस"
description: "एक मुख्य क्लास का प्रतिनिधित्व करता है जो दस्तावेज़ रेडैक्शन प्रक्रिया को नियंत्रित करता है, जिससे दस्तावेज़ खोलना, रेडैक्ट करना और सहेजना संभव होता है।"
type: docs
weight: 820
url: /hi/net/groupdocs.redaction/redactor/
---
## Redactor class

एक मुख्य क्लास का प्रतिनिधित्व करता है जो दस्तावेज़ रेडैक्शन प्रक्रिया को नियंत्रित करता है, जिससे दस्तावेज़ खोलना, रेडैक्ट करना और सहेजना संभव होता है।

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Constructors

| नाम | विवरण |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | [`Redactor`](../redactor) क्लास का नया इंस्टेंस स्ट्रीम का उपयोग करके इनिशियलाइज़ करता है। |
| [Redactor](redactor#constructor_3)(string) | [`Redactor`](../redactor) क्लास का नया इंस्टेंस फ़ाइल पाथ का उपयोग करके इनिशियलाइज़ करता है। |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | पासवर्ड-प्रोटेक्टेड दस्तावेज़ के लिए स्ट्रीम का उपयोग करके [`Redactor`](../redactor) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | पासवर्ड-संरक्षित दस्तावेज़ के लिए उसके पथ का उपयोग करके [`Redactor`](../redactor) वर्ग का नया उदाहरण आरंभ करता है। |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | स्ट्रीम और सेटिंग्स का उपयोग करके पासवर्ड-संरक्षित दस्तावेज़ के लिए [`Redactor`](../redactor) वर्ग का नया उदाहरण आरंभ करता है। |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | उसके पथ और सेटिंग्स का उपयोग करके पासवर्ड-संरक्षित दस्तावेज़ के लिए [`Redactor`](../redactor) वर्ग का नया उदाहरण आरंभ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | दस्तावेज़ पर एक रेडैक्शन लागू करता है। |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | दस्तावेज़ पर एक रेडैक्शन नीति लागू करता है। |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | दस्तावेज़ पर रेडैक्शन का एक सेट लागू करता है। |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | संसाधनों को मुक्त करता है। |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | दिए गए इमेज फ़ॉर्मेट में विशिष्ट पृष्ठों की प्रीव्यू इमेज बनाता है। |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | दस्तावेज़ की सामान्य जानकारी प्राप्त करता है - आकार, पृष्ठ संख्या, आदि। |
| [Save](../../groupdocs.redaction/redactor/save#save)() | दस्तावेज़ को फ़ाइल में निम्न विकल्पों के साथ सहेजता है: AddSuffix = true, RasterizeToPDF = true। |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | दस्तावेज़ को फ़ाइल में सहेजता है। |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | दस्तावेज़ को निर्दिष्ट स्ट्रीम में सहेजता है। |

### टिप्पणियाँ

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### उदाहरण

निम्न उदाहरण दस्तावेज़ पर एकल रेडैक्शन लागू करने को दर्शाता है।

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

निम्न उदाहरण दस्तावेज़ पर रेडैक्शन की सूची लागू करने को दर्शाता है।

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... अन्य रेडैक्शन
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, यदि कम से कम एक रेडैक्शन विफल हो गया
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

निम्नलिखित उदाहरण दर्शाता है कि कैसे एक निर्दिष्ट इनबाउंड फ़ोल्डर के भीतर सभी फ़ाइलों पर रेडैक्शन नीति लागू की जाए, और सफलतापूर्वक अपडेट की गई फ़ाइलों और विफल फ़ाइलों के लिए आउटबाउंड फ़ोल्डरों में से एक में सहेजा जाए।

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

निम्न उदाहरण LoadOptions का उपयोग करके पासवर्ड-संरक्षित दस्तावेज़ों को खोलने का तरीका दर्शाता है।

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // यहाँ हम रेडैक्शन करने के लिए दस्तावेज़ इंस्टेंस का उपयोग कर सकते हैं।
}
```

निम्नलिखित उदाहरण दिखाता है कि SaveOptions का उपयोग करके दस्तावेज़ को कैसे सहेजा जाए।

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // दस्तावेज़ रिडैक्शन यहाँ जाता है
       // ...
    
       // डिफ़ॉल्ट विकल्पों के साथ दस्तावेज़ सहेजें (पृष्ठों को छवियों में बदलें, PDF के रूप में सहेजें)
       redactor.Save();
    
       // मूल फ़ाइल को अधिलेखित करते हुए मूल फ़ॉर्मेट में दस्तावेज़ सहेजें
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // दस्तावेज़ को मूल फ़ॉर्मेट में "*_Redacted.*" फ़ाइल में सहेजें
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // दस्तावेज़ को "*_AnyText.*" (उदाहरण के लिए "AnyText" के बजाय टाइमस्टैम्प) के फ़ाइल नाम में रास्टराइज़ेशन के बिना सहेजें
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### साथ ही देखें

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
