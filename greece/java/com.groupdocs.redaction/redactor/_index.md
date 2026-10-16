---
title: "Redactor"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια κύρια κλάση που ελέγχει τη διαδικασία επεξεργασίας εγγράφων, επιτρέποντας το άνοιγμα, την επεξεργασία και την αποθήκευση εγγράφων."
type: docs
weight: 16
url: /el/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Αντιπροσωπεύει την κύρια κλάση που ελέγχει τη διαδικασία απόκρυψης εγγράφων, επιτρέποντας το άνοιγμα, την απόκρυψη και την αποθήκευση εγγράφων.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | Αρχικοποιεί μια νέα αντιπροσωπεία του |
Redactor
κλάση που χρησιμοποιεί διαδρομή αρχείου.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Αρχικοποιεί μια νέα αντιπροσωπεία του |
Redactor
κλάση που χρησιμοποιεί ροή.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Αρχικοποιεί μια νέα αντιπροσωπεία του |
Redactor
κλάση για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας τη διαδρομή του.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Αρχικοποιεί μια νέα αντιπροσωπεία του |
Redactor
κλάση για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας τη διαδρομή του και τις ρυθμίσεις.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Αρχικοποιεί μια νέα αντιπροσωπεία του |
Redactor
κλάση για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας ροή.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Αρχικοποιεί μια νέα αντιπροσωπεία του |
Redactor
κλάση για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας ροή και ρυθμίσεις.
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [close()](#close--) | Απελευθερώνει πόρους. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Εφαρμόζει μια επεξεργασία στο έγγραφο. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Εφαρμόζει ένα σύνολο επεξεργασιών στο έγγραφο. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Εφαρμόζει μια πολιτική επεξεργασίας στο έγγραφο. |
|
|  | [save()](#save--) | Αποθηκεύει το έγγραφο σε αρχείο με τις ακόλουθες επιλογές: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Αποθηκεύει το έγγραφο σε αρχείο. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | Αποθηκεύει το έγγραφο σε ροή. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | Αποθηκεύει το έγγραφο σε ροή. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Αποθηκεύει το έγγραφο σε ροή, συμπεριλαμβανομένης της προσαρμοσμένης τοποθεσίας. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Λαμβάνει τις γενικές πληροφορίες σχετικά με το έγγραφο - μέγεθος, αριθμός σελίδων κ.λπ. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Αρχικοποιεί μια νέα αντιπροσωπεία του
Redactor
κλάση που χρησιμοποιεί διαδρομή αρχείου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Διαδρομή προς το αρχείο |


Το παρακάτω παράδειγμα δείχνει πώς να ανοίξετε ένα έγγραφο για επεξεργασία.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// Εδώ μπορούμε να χρησιμοποιήσουμε το αντικείμενο document για να εκτελέσουμε τις επεμβάσεις
Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ExactPhraseRedaction σε λειτουργία χωρίς διάκριση πεζών-κεφαλαίων.
Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ExactPhraseRedaction σε λειτουργία χωρίς διάκριση πεζών-κεφαλαίων.
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Αρχικοποιεί μια νέα αντιπροσωπεία του
Redactor
κλάση για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας τη διαδρομή του.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Διαδρομή προς το αρχείο. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Επιλογές, συμπεριλαμβανομένου κωδικού πρόσβασης. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Αρχικοποιεί μια νέα αντιπροσωπεία του
Redactor
κλάση για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας τη διαδρομή του και τις ρυθμίσεις.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Διαδρομή προς το αρχείο. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Επιλογές που εξαρτώνται από το αρχείο, συμπεριλαμβανομένου κωδικού πρόσβασης. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία επεξαίρεσης. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Αρχικοποιεί μια νέα αντιπροσωπεία του
Redactor
κλάση για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.InputStream | Ροή εισόδου προέλευσης. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Επιλογές, συμπεριλαμβανομένου κωδικού πρόσβασης. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Αρχικοποιεί μια νέα αντιπροσωπεία του
Redactor
κλάση για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας ροή και ρυθμίσεις.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.InputStream | Ροή εισόδου προέλευσης. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Επιλογές, συμπεριλαμβανομένου κωδικού πρόσβασης. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία επεξαίρεσης. |
|

### close() {#close--}
```
public final void close()
```


Απελευθερώνει πόρους.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Εφαρμόζει μια επεξεργασία στο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Μία παρουσία του Redaction για εφαρμογή |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Εφαρμόζει ένα σύνολο επεξεργασιών στο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Μία σειρά από redactions για εφαρμογή |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Εφαρμόζει μια πολιτική επεξεργασίας στο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Redation πολιτική |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


Αποθηκεύει το έγγραφο σε αρχείο με τις ακόλουθες επιλογές: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - Διαδρομή προς το επεξεργασμένο έγγραφο

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Αποθηκεύει το έγγραφο σε αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Επιλογές για προσθήκη καταλήξεως ή rasterize |
|

**Returns:**
java.lang.String - Διαδρομή προς το επεξεργασμένο έγγραφο

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


Αποθηκεύει το έγγραφο σε ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.OutputStream | Ροή προορισμού |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


Αποθηκεύει το έγγραφο σε ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.OutputStream | Ροή προορισμού |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Επιλογές αποθήκευσης |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Αποθηκεύει το έγγραφο σε ροή, συμπεριλαμβανομένης της προσαρμοσμένης τοποθεσίας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | java.io.OutputStream | Ροή προορισμού |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Επιλογές για rasterize ή όχι και για καθορισμό σελίδων για rasterization |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Ρυθμίσεις ιδιοτήτων εικόνας και εύρους σελίδων |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Λαμβάνει τις γενικές πληροφορίες σχετικά με το έγγραφο - μέγεθος, αριθμός σελίδων κ.λπ.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

