---
title: Load
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Φορτώνει μια παρουσία τουRedactionPolicygroupdocs.redaction/redactionpolicy από μια διαδρομή αρχείου.
type: docs
weight: 20
url: /el/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Φορτώνει μια παρουσία του[`RedactionPolicy`](../../redactionpolicy) από μια διαδρομή αρχείου.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Διαδρομή προς το αρχείο XML |

### Επιστρεφόμενη Αξία

Πολιτική επιμέλειας

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς μπορείτε να εφαρμόσετε μια πολιτική επεξεργασίας σε όλα τα αρχεία ενός δεδομένου εισερχόμενου φακέλου και να αποθηκεύσετε σε έναν από τους φακέλους εξερχόμενων - για αρχεία που ενημερώθηκαν με επιτυχία και για αρχεία που απέτυχαν.

Το ακόλουθο παράδειγμα περιέχει ένα δείγμα αρχείου πολιτικής XML με δείγματα ρυθμίσεων για όλους τους τύπους διορθώσεων.

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

### Δείτε επίσης

* class [RedactionPolicy](../../redactionpolicy)
* χώρος ονομάτων [GroupDocs.Redaction](../../redactionpolicy)
* συνέλευση [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Φορτώνει μια παρουσία του[`RedactionPolicy`](../../redactionpolicy) από μια ροή.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| input | Stream | Ροή που περιέχει διαμόρφωση XML |

### Επιστρεφόμενη Αξία

Πολιτική επιμέλειας

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς μπορείτε να εφαρμόσετε μια πολιτική επεξεργασίας σε όλα τα αρχεία ενός δεδομένου εισερχόμενου φακέλου και να αποθηκεύσετε σε έναν από τους φακέλους εξερχόμενων - για αρχεία που ενημερώθηκαν με επιτυχία και για αρχεία που απέτυχαν.

Το ακόλουθο παράδειγμα περιέχει ένα δείγμα αρχείου πολιτικής XML με δείγματα ρυθμίσεων για όλους τους τύπους διορθώσεων.

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

### Δείτε επίσης

* class [RedactionPolicy](../../redactionpolicy)
* χώρος ονομάτων [GroupDocs.Redaction](../../redactionpolicy)
* συνέλευση [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
