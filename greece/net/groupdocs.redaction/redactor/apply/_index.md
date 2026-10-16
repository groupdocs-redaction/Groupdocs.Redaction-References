---
title: "Εφαρμογή"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Εφαρμόζει μια απόκρυψη στο έγγραφο."
type: docs
weight: 20
url: /el/net/groupdocs.redaction/redactor/apply/
---
## Apply(Redaction) {#apply}

Εφαρμόζει μια απόκρυψη στο έγγραφο.

```csharp
public RedactorChangeLog Apply(Redaction redaction)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| redaction | Redaction | Μία παρουσία του [`Redaction`](../../redaction) για εφαρμογή |

### Τιμή Επιστροφής

Επιτυχία ή αποτυχία και μήνυμα σφάλματος σε αυτήν την περίπτωση.

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

### Δείτε επίσης

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(Redaction[]) {#apply_2}

Εφαρμόζει ένα σύνολο αποκρύψεων στο έγγραφο.

```csharp
public RedactorChangeLog Apply(Redaction[] redactions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| redactions | Redaction[] | Ένας πίνακας των redactions για εφαρμογή |

### Τιμή Επιστροφής

Επιτυχία ή αποτυχία και μήνυμα σφάλματος σε αυτήν την περίπτωση.

### Παραδείγματα

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

### Δείτε επίσης

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(RedactionPolicy) {#apply_1}

Εφαρμόζει μια πολιτική απόκρυψης στο έγγραφο.

```csharp
public RedactorChangeLog Apply(RedactionPolicy policy)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πολιτική | RedactionPolicy | Πολιτική διαγραφής |

### Τιμή Επιστροφής

Επιτυχία ή αποτυχία και μήνυμα σφάλματος σε αυτήν την περίπτωση.

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

### Δείτε επίσης

* class [RedactorChangeLog](../../redactorchangelog)
* class [RedactionPolicy](../../redactionpolicy)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
