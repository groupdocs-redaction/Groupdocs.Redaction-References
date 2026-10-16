---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αναπαριστά το φίλτρο επεξεργασίας που ορίζει το εύρος σελίδων μέσα σε ένα έγγραφο για την εφαρμογή επεξεργασίας."
type: docs
weight: 24
url: /el/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

Αντιπροσωπεύει φίλτρο διαγραφής, ορίζοντας εύρος σελίδων μέσα σε ένα έγγραφο για την εφαρμογή διαγραφής.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης RemovePageRedaction. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | Λαμβάνει τη θέση αναφοράς αναζήτησης, την αρχή ή το τέλος ενός εγγράφου. |
|
|  | [getIndex()](#getIndex--) | Λαμβάνει τον δείκτη θέσης έναρξης (0‑βάση). |
|
|  | [getCount()](#getCount--) | Λαμβάνει τον αριθμό των σελίδων προς αφαίρεση. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | Ελέγχει εάν αυτή η περιοχή σελίδων του φίλτρου περιέχει τη δοθείσα σελίδα. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης RemovePageRedaction.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | Θέση αναφοράς αναζήτησης, η αρχή ή το τέλος ενός εγγράφου |
|
|  | δείκτης | int | Δείκτης θέσης έναρξης (0‑βάση) |
|
|  | αριθμός | int | Αριθμός σελίδων προς αφαίρεση |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


Λαμβάνει τη θέση αναφοράς αναζήτησης, την αρχή ή το τέλος ενός εγγράφου.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Λαμβάνει τον δείκτη θέσης έναρξης (0‑βάση).


**Returns:**
int - Αρχικός δείκτης θέσης (0-based).

### getCount() {#getCount--}
```
public final int getCount()
```


Λαμβάνει τον αριθμό των σελίδων προς αφαίρεση.


**Returns:**
int - Ο αριθμός σελίδων προς αφαίρεση.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


Ελέγχει εάν αυτή η περιοχή σελίδων του φίλτρου περιέχει τη δοθείσα σελίδα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pageIndex | int | δείκτης της σελίδας (zero-bazed) |
|
|  | pageCount | int | συνολικός αριθμός σελίδων |
|

**Returns:**
boolean - true, εάν αυτό το φάσμα φίλτρου περιέχει σελίδα

