---
title: "Load"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Φορτώνει ένα αντίτυπο του RedactionPolicygroupdocs.redaction/redactionpolicy από διαδρομή αρχείου."
type: docs
weight: 20
url: /el/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Φορτώνει ένα αντίτυπο του [`RedactionPolicy`](../../redactionpolicy) από διαδρομή αρχείου.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Διαδρομή προς αρχείο XML |

### Τιμή Επιστροφής

Πολιτική διαγραφής

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εφαρμόσετε μια πολιτική διαγραφής σε όλα τα αρχεία μέσα σε έναν συγκεκριμένο φάκελο εισόδου και να τα αποθηκεύσετε σε έναν από τους φακέλους εξόδου — για αρχεία που ενημερώθηκαν επιτυχώς και για αποτυχημένα.

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

Το παρακάτω παράδειγμα περιέχει ένα δείγμα αρχείου πολιτικής XML με παραδείγματα ρυθμίσεων για όλους τους τύπους διαγραφών.

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
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Φορτώνει ένα αντίτυπο του [`RedactionPolicy`](../../redactionpolicy) από ροή.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| είσοδος | Stream | Ροή που περιέχει ρυθμίσεις XML |

### Τιμή Επιστροφής

Πολιτική διαγραφής

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εφαρμόσετε μια πολιτική διαγραφής σε όλα τα αρχεία μέσα σε έναν συγκεκριμένο φάκελο εισόδου και να τα αποθηκεύσετε σε έναν από τους φακέλους εξόδου — για αρχεία που ενημερώθηκαν επιτυχώς και για αποτυχημένα.

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

Το παρακάτω παράδειγμα περιέχει ένα δείγμα αρχείου πολιτικής XML με παραδείγματα ρυθμίσεων για όλους τους τύπους διαγραφών.

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
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
