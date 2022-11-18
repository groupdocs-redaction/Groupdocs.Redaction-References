---
title: Load
second_title: GroupDocs.Redaction لمرجع .NET API
description: يتم تحميل مثيلRedactionPolicygroupdocs.redaction/redactionpolicy من مسار ملف.
type: docs
weight: 20
url: /ar/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

يتم تحميل مثيل[`RedactionPolicy`](../../redactionpolicy) من مسار ملف.

```csharp
public static RedactionPolicy Load(string filePath)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| filePath | String | مسار ملف XML |

### قيمة الإرجاع

سياسة التنقيح

### أمثلة

يوضح المثال التالي كيفية تطبيق سياسة التنقيح على جميع الملفات داخل مجلد وارد معين ، وحفظها في أحد المجلدات الصادرة - للملفات التي تم تحديثها بنجاح والملفات الفاشلة.

يحتوي المثال التالي على نموذج لملف سياسة XML مع نماذج تكوينات لجميع أنواع التنقيحات.

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
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction ">;
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

### أنظر أيضا

* class [RedactionPolicy](../../redactionpolicy)
* مساحة الاسم [GroupDocs.Redaction](../../redactionpolicy)
* المجسم [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

يتم تحميل مثيل[`RedactionPolicy`](../../redactionpolicy) من تيار .

```csharp
public static RedactionPolicy Load(Stream input)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| input | Stream | دفق يحتوي على تكوين XML |

### قيمة الإرجاع

سياسة التنقيح

### أمثلة

يوضح المثال التالي كيفية تطبيق سياسة التنقيح على جميع الملفات داخل مجلد وارد معين ، وحفظها في أحد المجلدات الصادرة - للملفات التي تم تحديثها بنجاح والملفات الفاشلة.

يحتوي المثال التالي على نموذج لملف سياسة XML مع نماذج تكوينات لجميع أنواع التنقيحات.

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
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction ">;
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

### أنظر أيضا

* class [RedactionPolicy](../../redactionpolicy)
* مساحة الاسم [GroupDocs.Redaction](../../redactionpolicy)
* المجسم [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
