---
title: Redactor
second_title: .NET API संदर्भ के लिए GroupDocs.Redaction
description: एक मुख्य वर्ग क प्रतनधत्व करत है ज दस्तवेज़ संपदन प्रक्रय क नयंत्रत करत है दस्तवेज़ं क खलने संपदत करने और सहेजने क अनुमत देत है
type: docs
weight: 660
url: /hi/net/groupdocs.redaction/redactor/
---
## Redactor class

एक मुख्य वर्ग का प्रतिनिधित्व करता है जो दस्तावेज़ संपादन प्रक्रिया को नियंत्रित करता है, दस्तावेज़ों को खोलने, संपादित करने और सहेजने की अनुमति देता है।

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | का एक नया उदाहरण शुरू करता है[`Redactor`](../redactor) धारा का उपयोग कर कक्षा। |
| [Redactor](redactor#constructor_3)(string) | का एक नया उदाहरण शुरू करता है[`Redactor`](../redactor) वर्ग फ़ाइल पथ. का उपयोग कर |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | का एक नया उदाहरण शुरू करता है[`Redactor`](../redactor) स्ट्रीम. का उपयोग करके पासवर्ड से सुरक्षित दस्तावेज़ के लिए वर्ग |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | का एक नया उदाहरण शुरू करता है[`Redactor`](../redactor) अपने पथ का उपयोग करते हुए पासवर्ड-सुरक्षित दस्तावेज़ के लिए क्लास . |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | का एक नया उदाहरण शुरू करता है[`Redactor`](../redactor)स्ट्रीम और सेटिंग का उपयोग करके पासवर्ड से सुरक्षित दस्तावेज़ के लिए क्लास. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | का एक नया उदाहरण शुरू करता है[`Redactor`](../redactor) अपने पथ और सेटिंग्स का उपयोग करके पासवर्ड-सुरक्षित दस्तावेज़ के लिए वर्ग। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | दस्तावेज़ में संशोधन लागू करता है। |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | दस्तावेज़ में संशोधन नीति लागू करता है। |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | दस्तावेज़ में संशोधनों का एक सेट लागू करता है। |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | संसाधन जारी करता है। |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | दिए गए छवि प्रारूप में विशिष्ट पृष्ठों की पूर्वावलोकन छवियां उत्पन्न करता है. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | दस्तावेज़ के बारे में सामान्य जानकारी प्राप्त करता है - आकार, पृष्ठ संख्या, आदि. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | निम्नलिखित विकल्पों के साथ दस्तावेज़ को फ़ाइल में सहेजता है: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | दस्तावेज़ को फ़ाइल में सहेजता है. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | कस्टम स्थान सहित दस्तावेज़ को स्ट्रीम में सहेजता है. |

### टिप्पणियों

**और अधिक जानें**

* कटौती लागू करने के बारे में अधिक विवरण: [सुधार मूल बातें](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* अधिक उन्नत संपादन विषय: [उन्नत उपयोग](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### उदाहरण

निम्न उदाहरण दस्तावेज़ में एकल संशोधन लागू करने को प्रदर्शित करता है।

निम्नलिखित उदाहरण दस्तावेज़ में कटौती की सूची को लागू करने का प्रदर्शन करता है।

निम्न उदाहरण प्रदर्शित करता है कि किसी दिए गए इनबाउंड फ़ोल्डर में सभी फ़ाइलों के लिए एक सुधार नीति कैसे लागू की जाए, और आउटबाउंड फ़ोल्डरों में से किसी एक को कैसे सहेजा जाए - सफलतापूर्वक अपडेट की गई फ़ाइलों के लिए और विफल फ़ाइलों के लिए।

निम्न उदाहरण दर्शाता है कि LoadOptions का उपयोग करके पासवर्ड-सुरक्षित दस्तावेज़ कैसे खोलें।

निम्न उदाहरण दर्शाता है कि कैसे SaveOptions का उपयोग करके दस्तावेज़ को सहेजना है।

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

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... अन्य कटौती
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // असत्य, यदि कम से कम एक सुधार विफल हुआ
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

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

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // यहां हम रिडक्शन करने के लिए डॉक्यूमेंट इंस्टेंस का उपयोग कर सकते हैं
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // दस्तावेज़ सुधार यहां जाता है
       // ...
    
       // दस्तावेज़ को डिफ़ॉल्ट विकल्पों के साथ सहेजें (पृष्ठों को छवियों में बदलें, पीडीएफ के रूप में सहेजें)
       redactor.Save();
    
       // मूल फ़ाइल को ओवरराइट करने के लिए दस्तावेज़ को मूल स्वरूप में सहेजें
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // दस्तावेज़ को मूल स्वरूप में "*_Redacted.*" फ़ाइल में सहेजें
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // दस्तावेज़ को "*_AnyText.*" में सहेजें (उदाहरण के लिए "AnyText" के बजाय टाइमस्टैम्प) बिना रेखांकन के इसके फ़ाइल नाम में
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### यह सभी देखें

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* नाम स्थान [GroupDocs.Redaction](../../groupdocs.redaction)
* सभा [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
