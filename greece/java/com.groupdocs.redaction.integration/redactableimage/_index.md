---
title: "RedactableImage"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Παρέχει διεπαφή για όλες τις λειτουργίες διαγραφής ραστερ εικόνων."
type: docs
weight: 14
url: /el/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Παρέχει διεπαφή για όλες τις λειτουργίες διαγραφής ραστερ εικόνων.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Δημιουργεί μια νέα παρουσία χρησιμοποιώντας ένα αντικείμενο, που υλοποιεί |
IImageFormatInstance
διασύνδεση.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Δημιουργεί μια νέα παρουσία χρησιμοποιώντας ένα αντικείμενο, που υλοποιεί |
IMultipleAreaRedactable
διασύνδεση.
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Ανακτά μια ροή με το πραγματικό περιεχόμενο της εικόνας. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Αποκρύπτει πολλαπλές περιοχές εικόνας ταυτόχρονα με το ίδιο χρώμα. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Αντικαθιστά την περιοχή σε δεδομένο σημείο με ένα ορθογώνιο συγκεκριμένου χρώματος και μεγέθους. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Δημιουργεί μια νέα παρουσία χρησιμοποιώντας ένα αντικείμενο, που υλοποιεί
IImageFormatInstance
διασύνδεση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | Μια παρουσία, που υλοποιεί τη διεπαφή IImageFormatInstance |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Δημιουργεί μια νέα παρουσία χρησιμοποιώντας ένα αντικείμενο, που υλοποιεί
IMultipleAreaRedactable
διασύνδεση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | Μια παρουσία, που υλοποιεί τη διεπαφή IMultipleAreaRedactable |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Ανακτά μια ροή με το πραγματικό περιεχόμενο της εικόνας.


**Returns:**
java.io.InputStream - Ροή, που περιέχει δεδομένα εικόνας

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Αποκρύπτει πολλαπλές περιοχές εικόνας ταυτόχρονα με το ίδιο χρώμα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ορθογώνια | java.awt.Rectangle[] | Ένας πίνακας περιοχών ορθογωνίων |
|
|  | boxColor | java.awt.Color | Χρώμα για γέμισμα των περιοχών |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Αντικαθιστά την περιοχή σε δεδομένο σημείο με ένα ορθογώνιο συγκεκριμένου χρώματος και μεγέθους.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Συντεταγμένες επάνω-αριστερού γωνίας της γεμισμένης περιοχής |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Ρυθμίσεις χρώματος και μεγέθους |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

