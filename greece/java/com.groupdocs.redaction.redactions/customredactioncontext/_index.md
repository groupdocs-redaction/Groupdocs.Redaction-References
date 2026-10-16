---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Παρέχει δεδομένα εισόδου για ."
type: docs
weight: 13
url: /el/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Παρέχει δεδομένα εισόδου για [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Λαμβάνει τον αριθμό σελίδας του ταιριασμένου τμήματος, όταν είναι διαθέσιμο. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Ορίζει τον αριθμό σελίδας του ταιριασμένου τμήματος. |
|
|  | [getText()](#getText--) | Λαμβάνει το κείμενο που ταιριάζει για απόσπασμα. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Ορίζει το κείμενο που ταιριάζει για απόσπασμα. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Λαμβάνει τον αριθμό σελίδας του ταιριασμένου τμήματος, όταν είναι διαθέσιμο.


**Returns:**
int - Ο αριθμός σελίδας, ή μια τιμή ειδική για τη μορφή εάν η σελίδα δεν είναι γνωστή.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Ορίζει τον αριθμό σελίδας του ταιριασμένου τμήματος.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο αριθμός σελίδας. |
|

### getText() {#getText--}
```
public final String getText()
```


Λαμβάνει το κείμενο που ταιριάζει για απόσπασμα.


**Returns:**
java.lang.String - Το ταιριασμένο κείμενο.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Ορίζει το κείμενο που ταιριάζει για απόσπασμα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Το ταιριασμένο κείμενο. |
|

