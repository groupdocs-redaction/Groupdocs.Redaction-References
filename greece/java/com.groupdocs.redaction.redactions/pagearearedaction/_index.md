---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια σύνθετη κειμενική διαγραφή που επηρεάζει εικόνες κειμένου και σημειώσεις σε μια περιοχή της σελίδας."
type: docs
weight: 23
url: /el/java/com.groupdocs.redaction.redactions/pagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction), [com.groupdocs.redaction.redactions.RegexRedaction](../../com.groupdocs.redaction.redactions/regexredaction)
```
public class PageAreaRedaction extends RegexRedaction
```

Αντιπροσωπεύει μια σύνθετη κειμενική διαγραφή που επηρεάζει κείμενο, εικόνες και σημειώσεις σε μια περιοχή της σελίδας.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](../https://docs.groupdocs.com/redaction/java/use-page-area-redaction/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης PageAreaRedaction. |
|
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης PageAreaRedaction. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getImageOptions()](#getImageOptions--) | Λαμβάνει το |
RegionReplacementOptions
επιλογές με χρώμα και παραμέτρους περιοχής.
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Εφαρμόζει τη διαγραφή σε ένα δεδομένο αντικείμενο μορφής. |
|
### PageAreaRedaction(Pattern regex, ReplacementOptions options) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης PageAreaRedaction.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Κανονική έκφραση για αναζήτηση και αντικατάσταση |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Επιλογές αντικατάστασης (κειμενικές, χρώματος) |
|

### PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης PageAreaRedaction.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | regex | java.util.regex.Pattern | Κανονική έκφραση για αναζήτηση και αντικατάσταση |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Επιλογές αντικατάστασης (κειμενικές, χρώματος) |
|
|  | imageOptions | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Επιλογές αντικατάστασης (περιοχή εικόνας) |
|

### getImageOptions() {#getImageOptions--}
```
public final RegionReplacementOptions getImageOptions()
```


Λαμβάνει το
RegionReplacementOptions
επιλογές με χρώμα και παραμέτρους περιοχής.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

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

