---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια κειμενική διαγραφή που αναζητά και αντικαθιστά κείμενο στο έγγραφο ταιριάζοντας με την παρεχόμενη κανονική έκφραση."
type: docs
weight: 28
url: /el/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Αντιπροσωπεύει μια κειμενική διαγραφή που αναζητά και αντικαθιστά κείμενο στο έγγραφο ταιριάζοντας με την παρεχόμενη κανονική έκφραση.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης RegexRedaction. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης RegexRedaction. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Λαμβάνει την κανονική έκφραση για αντιστοίχιση. |
|
|  | [getDescription()](#getDescription--) | Επιστρέφει μια συμβολοσειρά που περιγράφει τη διαγραφή και τις παραμέτρους της. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Εφαρμόζει τη διαγραφή σε ένα δεδομένο αντικείμενο μορφής. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης RegexRedaction.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | πρότυπο | java.lang.String | Κανονική έκφραση για αναζήτηση και αντικατάσταση |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Επιλογές αντικατάστασης (κειμενικές, χρώματος) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης RegexRedaction.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Κανονική έκφραση για αναζήτηση και αντικατάσταση |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Επιλογές αντικατάστασης (κειμενικές, χρώματος) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Λαμβάνει την κανονική έκφραση για αντιστοίχιση.


**Returns:**
java.util.regex.Pattern - Η κανονική έκφραση για αντιστοίχιση.

### getDescription() {#getDescription--}
```
public String getDescription()
```


Επιστρέφει μια συμβολοσειρά που περιγράφει τη διαγραφή και τις παραμέτρους της.


**Returns:**
java.lang.String - Κείμενο, που περιέχει το όνομα και τις παραμέτρους της διαγραφής.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Εφαρμόζει τη διαγραφή σε ένα δεδομένο αντικείμενο μορφής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Μία παρουσία ενός εγγράφου για εφαρμογή διαγραφής |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

