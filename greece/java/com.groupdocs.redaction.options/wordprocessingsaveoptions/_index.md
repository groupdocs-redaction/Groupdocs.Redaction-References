---
title: "WordprocessingSaveOptions"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Επιλογές αποθήκευσης επεξεργασίας κειμένου."
type: docs
weight: 15
url: /el/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Επιλογές αποθήκευσης επεξεργασίας κειμένου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | Συμμόρφωση OOXML για εφαρμογή κατά την αποθήκευση. |
|
| [setOoxmlCompliance(WordProcessingComplianceLevel value)](#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-) |  |
### WordprocessingSaveOptions() {#WordprocessingSaveOptions--}
```
public WordprocessingSaveOptions()
```


### getOoxmlCompliance() {#getOoxmlCompliance--}
```
public final WordProcessingComplianceLevel getOoxmlCompliance()
```


Συμμόρφωση OOXML για εφαρμογή κατά την αποθήκευση.  null  διατηρεί το αρχικό επίπεδο εγγράφου. Η επιλογή Strict δεν μπορεί να αποθηκευτεί ως Ecma άμεσα· χρησιμοποιήστε πρώτα το Transitional.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

