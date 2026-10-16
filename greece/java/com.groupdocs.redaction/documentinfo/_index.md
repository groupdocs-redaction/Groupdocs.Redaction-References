---
title: "DocumentInfo"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει πληροφορίες σχετικά με το έγγραφο."
type: docs
weight: 10
url: /el/java/com.groupdocs.redaction/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo)
```
public class DocumentInfo implements IDocumentInfo
```

Αναπαριστά πληροφορίες για το έγγραφο. Υλοποιεί τη διεπαφή IDocumentInfo. Δείτε
IDocumentInfo
για παραδείγματα.

*** ** * ** ***


**Learn more**

* [Get file info](../https://docs.groupdocs.com/redaction/java/get-file-info/)

<br />


## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFileType()](#getFileType--) | Λαμβάνει την περιγραφή της μορφής αρχείου. |
|
|  | [getPageCount()](#getPageCount--) | Λαμβάνει το συνολικό πλήθος σελίδων. |
|
|  | [getSize()](#getSize--) | Λαμβάνει το μέγεθος του εγγράφου σε bytes. |
|
|  | [getPages()](#getPages--) | Λαμβάνει τη λίστα πληροφοριών σελίδας. |
|
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Λαμβάνει την περιγραφή της μορφής αρχείου.


**Returns:**
[FileType](../../com.groupdocs.redaction/filetype) - The file format description.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Λαμβάνει το συνολικό πλήθος σελίδων.


**Returns:**
int - Το συνολικό πλήθος σελίδων.

### getSize() {#getSize--}
```
public final long getSize()
```


Λαμβάνει το μέγεθος του εγγράφου σε bytes.


**Returns:**
long - Το μέγεθος του εγγράφου σε bytes.

### getPages() {#getPages--}
```
public final List<PageInfo> getPages()
```


Λαμβάνει τη λίστα πληροφοριών σελίδας.


**Returns:**
java.util.List<com.groupdocs.redaction.PageInfo> - Η λίστα πληροφοριών σελίδας.

