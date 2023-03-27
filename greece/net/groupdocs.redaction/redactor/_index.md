---
title: Redactor
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Αντιπροσωπεύει μια κύρια κλάση που ελέγχει τη διαδικασία επεξεργασίας εγγράφων επιτρέποντας το άνοιγμα την επεξεργασία και την αποθήκευση εγγράφων.
type: docs
weight: 660
url: /el/net/groupdocs.redaction/redactor/
---
## Redactor class

Αντιπροσωπεύει μια κύρια κλάση που ελέγχει τη διαδικασία επεξεργασίας εγγράφων, επιτρέποντας το άνοιγμα, την επεξεργασία και την αποθήκευση εγγράφων.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../redactor) τάξη με χρήση ροής. |
| [Redactor](redactor#constructor_3)(string) | Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../redactor) κλάση χρησιμοποιώντας διαδρομή αρχείου. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../redactor) τάξη για ένα έγγραφο που προστατεύεται με κωδικό πρόσβασης με χρήση ροής. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../redactor) κλάση για ένα έγγραφο που προστατεύεται με κωδικό πρόσβασης χρησιμοποιώντας τη διαδρομή του. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../redactor)τάξη για ένα έγγραφο που προστατεύεται με κωδικό πρόσβασης χρησιμοποιώντας ροή και ρυθμίσεις. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../redactor) τάξη για ένα έγγραφο που προστατεύεται με κωδικό πρόσβασης χρησιμοποιώντας τη διαδρομή και τις ρυθμίσεις του. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Εφαρμόζει μια διόρθωση στο έγγραφο. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Εφαρμόζει μια πολιτική επεξεργασίας στο έγγραφο. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Εφαρμόζει ένα σύνολο διορθώσεων στο έγγραφο. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Απελευθερώνει πόρους. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε μια δεδομένη μορφή εικόνας. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Λαμβάνει τις γενικές πληροφορίες σχετικά με το έγγραφο - μέγεθος, πλήθος σελίδων κ.λπ. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Αποθηκεύει το έγγραφο σε ένα αρχείο με τις ακόλουθες επιλογές: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Αποθηκεύει το έγγραφο σε ένα αρχείο. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Αποθηκεύει το έγγραφο σε μια ροή, συμπεριλαμβανομένης της προσαρμοσμένης τοποθεσίας. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* Περισσότερες λεπτομέρειες σχετικά με την εφαρμογή διορθώσεων: [Βασικά στοιχεία διόρθωσης](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Πιο προηγμένα θέματα διόρθωσης: [Προηγμένη χρήση](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει την εφαρμογή μιας μεμονωμένης έκδοσης στο έγγραφο.

Το ακόλουθο παράδειγμα δείχνει την εφαρμογή μιας λίστας διορθώσεων στο έγγραφο.

Το ακόλουθο παράδειγμα δείχνει πώς μπορείτε να εφαρμόσετε μια πολιτική επεξεργασίας σε όλα τα αρχεία ενός δεδομένου εισερχόμενου φακέλου και να αποθηκεύσετε σε έναν από τους φακέλους εξερχόμενων - για αρχεία που ενημερώθηκαν με επιτυχία και για αρχεία που απέτυχαν.

Το ακόλουθο παράδειγμα δείχνει πώς να ανοίξετε έγγραφα που προστατεύονται με κωδικό πρόσβασης χρησιμοποιώντας το LoadOptions.

Το ακόλουθο παράδειγμα δείχνει πώς να αποθηκεύσετε ένα έγγραφο χρησιμοποιώντας το SaveOptions.

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
      // ... άλλες διασκευές
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // false, εάν τουλάχιστον μία διόρθωση απέτυχε
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
    // Εδώ μπορούμε να χρησιμοποιήσουμε το παράδειγμα εγγράφου για να εκτελέσουμε διορθώσεις
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Η επεξεργασία του εγγράφου πηγαίνει εδώ
       //...
    
       // Αποθήκευση του εγγράφου με προεπιλεγμένες επιλογές (μετατροπή σελίδων σε εικόνες, αποθήκευση ως PDF)
       redactor.Save();
    
       // Αποθηκεύστε το έγγραφο στην αρχική μορφή αντικαθιστώντας το αρχικό αρχείο
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Αποθηκεύστε το έγγραφο στο αρχείο "*_Redacted.*" στην αρχική μορφή
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Αποθηκεύστε το έγγραφο στο "*_AnyText.*" (π.χ. χρονική σήμανση αντί για "AnyText") στο όνομα του αρχείου του χωρίς ραστεροποίηση
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Δείτε επίσης

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* χώρος ονομάτων [GroupDocs.Redaction](../../groupdocs.redaction)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
