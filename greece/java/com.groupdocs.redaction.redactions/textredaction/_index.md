---
title: "TextRedaction"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια βασική αφηρημένη κλάση για κειμενικές διαγραφές εγγράφου."
type: docs
weight: 32
url: /el/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Αντιπροσωπεύει μια βασική αφηρημένη κλάση για κειμενικές διαγραφές εγγράφου.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Λαμβάνει το |
ReplacementOptions
παράδειγμα, που καθορίζει τον τύπο αντικατάστασης κειμένου.
|
|  | [getOcrConnector()](#getOcrConnector--) | Λαμβάνει το |
IOcrConnector
υλοποίηση, απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Ορίζει το |
IOcrConnector
υλοποίηση, απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Λαμβάνει το
ReplacementOptions
παράδειγμα, που καθορίζει τον τύπο αντικατάστασης κειμένου.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Λαμβάνει το
IOcrConnector
υλοποίηση, απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Ορίζει το
IOcrConnector
υλοποίηση, απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Η  IOcrConnector  υλοποίηση, απαιτείται για την εξαγωγή κειμένου από γραφικό περιεχόμενο. |
|

