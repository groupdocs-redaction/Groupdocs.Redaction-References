---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει το φίλτρο διαγραφής που ορίζει μια περιοχή μέσα σε μια σελίδα εγγράφου για την εφαρμογή διαγραφής."
type: docs
weight: 22
url: /el/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Αντιπροσωπεύει φίλτρο διαγραφής, ορίζοντας μια περιοχή μέσα σε μια σελίδα εγγράφου για την εφαρμογή διαγραφής.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης PageAreaFilter για τη διαγραφή συγκεκριμένης περιοχής. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Αποκτά το ορθογώνιο (θέση επάνω‑αριστερά και μέγεθος της περιοχής) σε μια σελίδα. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Ελέγχει αν αυτή η περιοχή φίλτρου έχει τομή με το δοσμένο ορθογώνιο. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης PageAreaFilter για τη διαγραφή συγκεκριμένης περιοχής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Συντεταγμένες περιοχής επάνω‑αριστερά |
|
|  | μέγεθος | java.awt.Dimension | Μέγεθος και χρώμα περιοχής |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Αποκτά το ορθογώνιο (θέση επάνω‑αριστερά και μέγεθος της περιοχής) σε μια σελίδα.


**Returns:**
java.awt.Rectangle - Το ορθογώνιο (θέση επάνω‑αριστερά και μέγεθος της περιοχής) σε μια σελίδα.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Ελέγχει αν αυτή η περιοχή φίλτρου έχει τομή με το δοσμένο ορθογώνιο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ορθογώνιο | java.awt.Rectangle | Ορθογώνιο για έλεγχο |
|

**Returns:**
boolean - true, αν αυτή η περιοχή φίλτρου έχει τομή

