---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Παρέχει επιλογές για τον καθορισμό απαιτήσεων και διαχειριστών ροής για τη δημιουργία προεπισκόπησης."
type: docs
weight: 11
url: /el/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Παρέχει επιλογές για τον καθορισμό απαιτήσεων και διαχειριστών ροής για τη δημιουργία προεπισκόπησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PreviewOptions, προκαλώντας το κλείσιμο της ροής εξόδου. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PreviewOptions, προκαλώντας την επιστροφή της ροής εξόδου στον πελάτη για περαιτέρω χρήση. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getWidth()](#getWidth--) | Λαμβάνει ή ορίζει το πλάτος προεπισκόπησης σελίδας. |
|
|  | [setWidth(int value)](#setWidth-int-) | Λαμβάνει ή ορίζει το πλάτος προεπισκόπησης σελίδας. |
|
|  | [getHeight()](#getHeight--) | Λαμβάνει ή ορίζει το ύψος προεπισκόπησης σελίδας. |
|
|  | [setHeight(int value)](#setHeight-int-) | Λαμβάνει ή ορίζει το ύψος προεπισκόπησης σελίδας. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Λαμβάνει ή ορίζει έναν πίνακα αριθμών σελίδων για δημιουργία προεπισκόπησης. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Λαμβάνει ή ορίζει έναν πίνακα αριθμών σελίδων για δημιουργία προεπισκόπησης. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Λαμβάνει ή ορίζει τη μορφή εικόνας προεπισκόπησης. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Λαμβάνει ή ορίζει τη μορφή εικόνας προεπισκόπησης. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Λαμβάνει ή ορίζει μια παρουσία του delegate δημιουργίας ροής σελίδας. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Λαμβάνει ή ορίζει μια παρουσία του delegate δημιουργίας ροής σελίδας. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Λαμβάνει ή ορίζει μια παρουσία του delegate ολοκλήρωσης προεπισκόπησης σελίδας. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Λαμβάνει ή ορίζει μια παρουσία του delegate ολοκλήρωσης προεπισκόπησης σελίδας. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PreviewOptions, προκαλώντας το κλείσιμο της ροής εξόδου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Δημιουργεί μια ροή για μια συγκεκριμένη προεπισκόπηση σελίδας |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PreviewOptions, προκαλώντας την επιστροφή της ροής εξόδου στον πελάτη για περαιτέρω χρήση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Δημιουργεί μια ροή για μια συγκεκριμένη προεπισκόπηση σελίδας |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Ειδοποιεί ότι η δημιουργία προεπισκόπησης σελίδας ολοκληρώθηκε και λαμβάνει τη ροή εξόδου |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Λαμβάνει ή ορίζει το πλάτος προεπισκόπησης σελίδας.


**Returns:**
int - Πλάτος προεπισκόπησης σελίδας.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Λαμβάνει ή ορίζει το πλάτος προεπισκόπησης σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Πλάτος προεπισκόπησης σελίδας. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Λαμβάνει ή ορίζει το ύψος προεπισκόπησης σελίδας.


**Returns:**
int - Ύψος προεπισκόπησης σελίδας.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Λαμβάνει ή ορίζει το ύψος προεπισκόπησης σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ύψος προεπισκόπησης σελίδας. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Λαμβάνει ή ορίζει έναν πίνακα αριθμών σελίδων για δημιουργία προεπισκόπησης.


**Returns:**
int[] - Ένας πίνακας αριθμών σελίδων για δημιουργία προεπισκόπησης.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Λαμβάνει ή ορίζει έναν πίνακα αριθμών σελίδων για δημιουργία προεπισκόπησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int[] | Ένας πίνακας αριθμών σελίδων για δημιουργία προεπισκόπησης. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Λαμβάνει ή ορίζει τη μορφή εικόνας προεπισκόπησης.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Λαμβάνει ή ορίζει τη μορφή εικόνας προεπισκόπησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Μορφή εικόνας προεπισκόπησης. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Λαμβάνει ή ορίζει μια παρουσία του delegate δημιουργίας ροής σελίδας.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Λαμβάνει ή ορίζει μια παρουσία του delegate δημιουργίας ροής σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Μια παρουσία του delegate δημιουργίας ροής σελίδας. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Λαμβάνει ή ορίζει μια παρουσία του delegate ολοκλήρωσης προεπισκόπησης σελίδας.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Λαμβάνει ή ορίζει μια παρουσία του delegate ολοκλήρωσης προεπισκόπησης σελίδας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Μια παρουσία του delegate ολοκλήρωσης προεπισκόπησης σελίδας. |
|

