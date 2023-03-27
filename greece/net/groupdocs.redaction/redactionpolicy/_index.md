---
title: RedactionPolicy
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Αντιπροσωπεύει μια πολιτική απολύμανσης η οποία περιέχει ένα σύνολο συγκεκριμένων διορθώσεων προς εφαρμογή.
type: docs
weight: 410
url: /el/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

Αντιπροσωπεύει μια πολιτική απολύμανσης, η οποία περιέχει ένα σύνολο συγκεκριμένων διορθώσεων προς εφαρμογή.

```csharp
public class RedactionPolicy
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Δημιουργεί μια νέα παρουσία της πολιτικής Redaction. |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | Δημιουργεί μια νέα παρουσία της πολιτικής Redaction με μια συγκεκριμένη λίστα διορθώσεων. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | Λαμβάνει έναν πίνακα με πλήρως διαμορφωμένες παραμέτρους[`Redaction`](../redaction) -προερχόμενες τάξεις. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | Φορτώνει μια παρουσία του[`RedactionPolicy`](../redactionpolicy) από μια ροή. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | Φορτώνει μια παρουσία του[`RedactionPolicy`](../redactionpolicy) από μια διαδρομή αρχείου. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | Αποθηκεύει την πολιτική επεξεργασίας σε μια ροή. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | Αποθηκεύει την πολιτική επεξεργασίας σε ένα αρχείο. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* Περισσότερες λεπτομέρειες σχετικά με τις πολιτικές: [Χρήση πολιτικών διόρθωσης](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* Περισσότερες λεπτομέρειες σχετικά με την εφαρμογή διορθώσεων: [Βασικά στοιχεία διόρθωσης](https://docs.groupdocs.com/redaction/net/redaction-basics/)

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

* χώρος ονομάτων [GroupDocs.Redaction](../../groupdocs.redaction)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->