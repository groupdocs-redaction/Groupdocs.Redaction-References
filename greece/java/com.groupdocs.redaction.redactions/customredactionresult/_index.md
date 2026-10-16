---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει ένα αποτέλεσμα που επιστρέφεται από ."
type: docs
weight: 14
url: /el/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Αντιπροσωπεύει ένα αποτέλεσμα που επιστρέφεται από [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getApply()](#getApply--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η αντικατάσταση πρέπει να εφαρμοστεί. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η αντικατάσταση πρέπει να εφαρμοστεί. |
|
|  | [getText()](#getText--) | Λαμβάνει το κείμενο αντικατάστασης που χρησιμοποιείται όταν το #getApply().getApply() είναι |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | Ορίζει το κείμενο αντικατάστασης που χρησιμοποιείται όταν το #getApply().getApply() είναι |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η αντικατάσταση πρέπει να εφαρμοστεί.


**Returns:**
boolean -  true  για αντικατάσταση του ταιριασμένου κειμένου με #getText().getText(); διαφορετικά,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η αντικατάσταση πρέπει να εφαρμοστεί.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | true  για εφαρμογή της αντικατάστασης; διαφορετικά,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


Λαμβάνει το κείμενο αντικατάστασης που χρησιμοποιείται όταν το #getApply().getApply() είναι
true
.


**Returns:**
java.lang.String - Το κείμενο αντικατάστασης.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Ορίζει το κείμενο αντικατάστασης που χρησιμοποιείται όταν το #getApply().getApply() είναι
true
.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Το κείμενο αντικατάστασης. |
|

