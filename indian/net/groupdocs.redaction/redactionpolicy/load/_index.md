---
title: "लोड"
second_title: "GroupDocs.Redaction के लिए .NET API रेफ़रेंस"
description: "फ़ाइल पथ से RedactionPolicygroupdocs.redaction/redactionpolicy का एक उदाहरण लोड करता है।"
type: docs
weight: 20
url: /hi/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

फ़ाइल पथ से [`RedactionPolicy`](../../redactionpolicy) का एक उदाहरण लोड करता है।

```csharp
public static RedactionPolicy Load(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | XML फ़ाइल का पथ |

### रिटर्न वैल्यू

रेडैक्शन नीति

### उदाहरण

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

निम्नलिखित उदाहरण में सभी प्रकार के रेडैक्शन के लिए नमूना कॉन्फ़िगरेशन के साथ एक सैंपल XML नीति फ़ाइल शामिल है।

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

### साथ ही देखें

* class [RedactionPolicy](../../redactionpolicy)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

स्ट्रीम से [`RedactionPolicy`](../../redactionpolicy) का एक उदाहरण लोड करता है।

```csharp
public static RedactionPolicy Load(Stream input)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| इनपुट | Stream | XML कॉन्फ़िगरेशन वाली स्ट्रीम |

### रिटर्न वैल्यू

रेडैक्शन नीति

### उदाहरण

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

निम्नलिखित उदाहरण में सभी प्रकार के रेडैक्शन के लिए नमूना कॉन्फ़िगरेशन के साथ एक सैंपल XML नीति फ़ाइल शामिल है।

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

### साथ ही देखें

* class [RedactionPolicy](../../redactionpolicy)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
