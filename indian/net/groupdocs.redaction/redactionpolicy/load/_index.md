---
title: Load
second_title: .NET API संदर्भ के लिए GroupDocs.Redaction
description: क उदहरण लड करत हैRedactionPolicygroupdocs.redaction/redactionpolicy फ़इल पथ से.
type: docs
weight: 20
url: /hi/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

का उदाहरण लोड करता है[`RedactionPolicy`](../../redactionpolicy) फ़ाइल पथ से.

```csharp
public static RedactionPolicy Load(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | एक्सएमएल फ़ाइल का पथ |

### प्रतिलाभ की मात्रा

सुधार नीति

### उदाहरण

निम्न उदाहरण प्रदर्शित करता है कि किसी दिए गए इनबाउंड फ़ोल्डर में सभी फ़ाइलों के लिए एक सुधार नीति कैसे लागू की जाए, और आउटबाउंड फ़ोल्डरों में से किसी एक को कैसे सहेजा जाए - सफलतापूर्वक अपडेट की गई फ़ाइलों के लिए और विफल फ़ाइलों के लिए।

निम्न उदाहरण में सभी प्रकार के सुधारों के लिए नमूना कॉन्फ़िगरेशन के साथ एक नमूना XML नीति फ़ाइल है।

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
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction" >
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase = "dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <cellColumnRedaction regularExpression = "(foo)bar1" replacement="[red1]" columnIndex="1" worksheetIndex="2" /> 
  <cellColumnRedaction regularExpression = "(foo)bar2" replacement="[red2]" wokrsheetName="Sample" /> 
  
  <eraseMetadataRedaction filter = "All" />
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
 <annotationRedaction regularExpression = "(anno1)" replacement="foobar" />  
 <deleteAnnotationRedaction regularExpression = "(anno2)" />

 <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
 <imageAreaRedaction pointX = "110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy>
```

### यह सभी देखें

* class [RedactionPolicy](../../redactionpolicy)
* नाम स्थान [GroupDocs.Redaction](../../redactionpolicy)
* सभा [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

का उदाहरण लोड करता है[`RedactionPolicy`](../../redactionpolicy) एक धारा से.

```csharp
public static RedactionPolicy Load(Stream input)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| input | Stream | XML कॉन्फ़िगरेशन वाली स्ट्रीम |

### प्रतिलाभ की मात्रा

सुधार नीति

### उदाहरण

निम्न उदाहरण प्रदर्शित करता है कि किसी दिए गए इनबाउंड फ़ोल्डर में सभी फ़ाइलों के लिए एक सुधार नीति कैसे लागू की जाए, और आउटबाउंड फ़ोल्डरों में से किसी एक को कैसे सहेजा जाए - सफलतापूर्वक अपडेट की गई फ़ाइलों के लिए और विफल फ़ाइलों के लिए।

निम्न उदाहरण में सभी प्रकार के सुधारों के लिए नमूना कॉन्फ़िगरेशन के साथ एक नमूना XML नीति फ़ाइल है।

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
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction" >
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase = "dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <cellColumnRedaction regularExpression = "(foo)bar1" replacement="[red1]" columnIndex="1" worksheetIndex="2" /> 
  <cellColumnRedaction regularExpression = "(foo)bar2" replacement="[red2]" wokrsheetName="Sample" /> 
  
  <eraseMetadataRedaction filter = "All" />
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
 <annotationRedaction regularExpression = "(anno1)" replacement="foobar" />  
 <deleteAnnotationRedaction regularExpression = "(anno2)" />

 <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
 <imageAreaRedaction pointX = "110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy>
```

### यह सभी देखें

* class [RedactionPolicy](../../redactionpolicy)
* नाम स्थान [GroupDocs.Redaction](../../redactionpolicy)
* सभा [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
