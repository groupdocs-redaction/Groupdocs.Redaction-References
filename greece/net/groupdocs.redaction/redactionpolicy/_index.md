---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αναπαριστά μια πολιτική εξομάλυνσης που περιέχει ένα σύνολο συγκεκριμένων αποκρύψεων προς εφαρμογή."
type: docs
weight: 500
url: /el/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

Αντιπροσωπεύει μια πολιτική εξαγνισμού, που περιέχει ένα σύνολο συγκεκριμένων απόκρυψεων προς εφαρμογή.

```csharp
public class RedactionPolicy
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Δημιουργεί ένα νέο αντικείμενο της Redaction policy. |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | Δημιουργεί ένα νέο αντικείμενο της Redaction policy με έναν συγκεκριμένο κατάλογο αποκρύψεων. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | Λαμβάνει έναν πίνακα πλήρως διαμορφωμένων κλάσεων που προέρχονται από το [`Redaction`](../redaction). |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | Φορτώνει ένα αντίτυπο του [`RedactionPolicy`](../redactionpolicy) από μια ροή. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | Φορτώνει ένα αντίτυπο του [`RedactionPolicy`](../redactionpolicy) από διαδρομή αρχείου. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | Αποθηκεύει την πολιτική διαγραφής σε μια ροή. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | Αποθηκεύει την πολιτική διαγραφής σε αρχείο. |

### Παρατηρήσεις

**Learn more**

* More details about policies: [Use of redaction policies](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)

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

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
