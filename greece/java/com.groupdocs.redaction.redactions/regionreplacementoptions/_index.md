---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει παραμέτρους χρώματος και περιοχής για αντικατάσταση περιοχής εικόνας."
type: docs
weight: 29
url: /el/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Αναπαριστά παραμέτρους χρώματος και περιοχής για αντικατάσταση περιοχής εικόνας. Δείτε
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RegionReplacementOptions της οποίας το μέγεθος ταιριάζει με το δεδομένο κείμενο. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Λαμβάνει το χρώμα για να γεμίσει την περιοχή που έχει αφαιρεθεί. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Ορίζει το χρώμα για να γεμίσει την περιοχή που έχει αφαιρεθεί. |
|
|  | [getSize()](#getSize--) | Λαμβάνει το ορθογώνιο με και ύψος. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Ορίζει το ορθογώνιο με και ύψος. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RegionReplacementOptions.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Χρώμα για γέμισμα της περιοχής |
|
|  | μέγεθος | java.awt.Dimension | Μέγεθος γεμισμένης περιοχής |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RegionReplacementOptions της οποίας το μέγεθος ταιριάζει με το δεδομένο κείμενο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Χρώμα για γέμισμα της περιοχής |
|
|  | font | java.awt.Font | Γραμματοσειρά αναμενόμενου κειμένου |
|
|  | expectedText | java.lang.String | Αναμενόμενο κείμενο |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Λαμβάνει το χρώμα για να γεμίσει την περιοχή που έχει αφαιρεθεί.


**Returns:**
java.awt.Color - Το χρώμα για γέμισμα της περιοχής που έχει αφαιρεθεί.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Ορίζει το χρώμα για να γεμίσει την περιοχή που έχει αφαιρεθεί.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.awt.Color | Το χρώμα για γέμισμα της περιοχής που έχει αφαιρεθεί. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Λαμβάνει το ορθογώνιο με και ύψος.


**Returns:**
java.awt.Dimension - Το ορθογώνιο με και ύψος.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Ορίζει το ορθογώνιο με και ύψος.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.awt.Dimension | Το ορθογώνιο με και ύψος. |
|

