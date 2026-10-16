---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια επεξεργασία που τοποθετεί χρωματιστό ορθογώνιο στην καθορισμένη περιοχή ενός εγγράφου εικόνας."
type: docs
weight: 18
url: /el/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Αντιπροσωπεύει μια επεξεργασία που τοποθετεί χρωματιστό ορθογώνιο στην καθορισμένη περιοχή ενός εγγράφου εικόνας.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ImageAreaRedaction για τη διαγραφή συγκεκριμένου μεγέθους περιοχής. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getOptions()](#getOptions--) | Λαμβάνει το |
RegionReplacementOptions
επιλογές με χρώμα και παραμέτρους περιοχής.
|
|  | [getTopLeft()](#getTopLeft--) | Λαμβάνει τη θέση πάνω-αριστερά της περιοχής προς αφαίρεση |
|
|  | [getDescription()](#getDescription--) | Επιστρέφει μια συμβολοσειρά που περιγράφει τη διαγραφή και τις παραμέτρους της. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Εφαρμόζει τη διαγραφή σε ένα δεδομένο αντικείμενο μορφής. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ImageAreaRedaction για τη διαγραφή συγκεκριμένου μεγέθους περιοχής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Συντεταγμένες περιοχής επάνω‑αριστερά |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Μέγεθος και χρώμα περιοχής |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Λαμβάνει το
RegionReplacementOptions
επιλογές με χρώμα και παραμέτρους περιοχής.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Λαμβάνει τη θέση πάνω-αριστερά της περιοχής προς αφαίρεση


**Returns:**
java.awt.Point - Η θέση πάνω-αριστερά της περιοχής προς αφαίρεση

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

