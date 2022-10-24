---
title: LoadOptions
second_title: GroupDocs.Redaction for Java API Reference
description: Provides options that will be used to open a file.
type: docs
weight: 10
url: /java/com.groupdocs.redaction.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Provides options that will be used to open a file.

--------------------

**Learn more**

 *  [Loading documents][]
 *  [Load from local disk][]
 *  [Load from stream][]
 *  [Load password-protected document][]

The following example demonstrates how to open password-protected document.

```

  LoadOptions loadOptions = new LoadOptions("mysecretpassword");
 try (Redactor redactor = new Redactor("PasswordProtected.pdf", loadOptions))
 {
     // work with document
 }
 
```


[Loading documents]: https://docs.groupdocs.com/redaction/java/loading-documents/
[Load from local disk]: https://docs.groupdocs.com/redaction/java/load-from-local-disc/
[Load from stream]: https://docs.groupdocs.com/redaction/java/load-from-stream/
[Load password-protected document]: https://docs.groupdocs.com/redaction/java/load-password-protected-file/
## Constructors

| Constructor | Description |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initializes a new instance of LoadOptions class. |
| [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Initializes a new instance of LoadOptions class with specified password. |
## Methods

| Method | Description |
| --- | --- |
| [getPassword()](#getPassword--) | Gets a password for password-protected documents. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Sets a password for password-protected documents. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initializes a new instance of LoadOptions class.

### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Initializes a new instance of LoadOptions class with specified password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password for protected files |

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Gets a password for password-protected documents.

**Returns:**
java.lang.String - A password for password-protected documents.
### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Sets a password for password-protected documents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | A password for password-protected documents. |

