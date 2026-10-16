---
title: "Redactor"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αναπαριστά την κύρια κλάση που ελέγχει τη διαδικασία επεξεργασίας εγγράφων, επιτρέποντας το άνοιγμα, την επεξεργασία και την αποθήκευση εγγράφων."
type: docs
weight: 820
url: /el/net/groupdocs.redaction/redactor/
---
## Redactor class

Αντιπροσωπεύει την κύρια κλάση που ελέγχει τη διαδικασία απόκρυψης εγγράφων, επιτρέποντας το άνοιγμα, την απόκρυψη και την αποθήκευση εγγράφων.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../redactor) χρησιμοποιώντας ροή. |
| [Redactor](redactor#constructor_3)(string) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../redactor) χρησιμοποιώντας διαδρομή αρχείου. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../redactor) για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας ροή. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../redactor) για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας τη διαδρομή του. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../redactor) για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας ροή και ρυθμίσεις. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../redactor) για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας τη διαδρομή του και τις ρυθμίσεις. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Εφαρμόζει μια απόκρυψη στο έγγραφο. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Εφαρμόζει μια πολιτική απόκρυψης στο έγγραφο. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Εφαρμόζει ένα σύνολο αποκρύψεων στο έγγραφο. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Απελευθερώνει πόρους. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Λαμβάνει τις γενικές πληροφορίες για το έγγραφο - μέγεθος, αριθμό σελίδων, κ.λπ. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Αποθηκεύει το έγγραφο σε αρχείο με τις ακόλουθες επιλογές: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Αποθηκεύει το έγγραφο σε αρχείο. |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | Αποθηκεύει το έγγραφο στην καθορισμένη ροή. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει την εφαρμογή μιας μόνο απόκρυψης στο έγγραφο.

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

Το παρακάτω παράδειγμα δείχνει την εφαρμογή λίστας αποκρύψεων στο έγγραφο.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... άλλες αποκρύψεις
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, εάν τουλάχιστον μια απόκρυψη απέτυχε
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

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

Το παρακάτω παράδειγμα δείχνει πώς να ανοίξετε έγγραφα προστατευμένα με κωδικό χρησιμοποιώντας LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Εδώ μπορούμε να χρησιμοποιήσουμε την παρουσία του εγγράφου για να εκτελέσουμε αποκρύψεις
}
```

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε ένα έγγραφο χρησιμοποιώντας το SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Η διαγραφή εγγράφου πηγαίνει εδώ
       // ...
    
       // Αποθηκεύστε το έγγραφο με τις προεπιλεγμένες επιλογές (μετατροπή σελίδων σε εικόνες, αποθήκευση ως PDF)
       redactor.Save();
    
       // Αποθηκεύστε το έγγραφο στην αρχική μορφή αντικαθιστώντας το αρχικό αρχείο
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Αποθηκεύστε το έγγραφο σε αρχείο "*_Redacted.*" στην αρχική μορφή
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Αποθηκεύστε το έγγραφο σε "*_AnyText.*" (π.χ. χρονική σήμανση αντί για "AnyText") στο όνομα αρχείου του χωρίς rasterization
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Δείτε επίσης

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
