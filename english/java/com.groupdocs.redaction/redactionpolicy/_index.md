---
title: RedactionPolicy
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a sanitization policy containing a set of specific redactions to apply.
type: docs
weight: 14
url: /java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Represents a sanitization policy, containing a set of specific redactions to apply.

--------------------

**Learn more**

 *  More details about policies: [Use of redaction policies][]
 *  More details about applying redactions: [Redaction basics][]


[Use of redaction policies]: https://docs.groupdocs.com/redaction/java/use-redaction-policies/
[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
## Constructors

| Constructor | Description |
| --- | --- |
| [RedactionPolicy()](#RedactionPolicy--) | Creates a new instance of Redaction policy. |
| [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Creates a new instance of Redaction policy with a specific list of redactions. |
## Methods

| Method | Description |
| --- | --- |
| [getRedactions()](#getRedactions--) | Gets an array of fully configured  Redaction -derived classes. |
| [load(String filePath)](#load-java.lang.String-) | Loads an instance of  RedactionPolicy  from a file path. |
| [load(InputStream input)](#load-java.io.InputStream-) | Loads an instance of  RedactionPolicy  from a stream. |
| [save(String filePath)](#save-java.lang.String-) | Saves the redaction policy to a file. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Saves the redaction policy to a stream. |
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Creates a new instance of Redaction policy.

### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Creates a new instance of Redaction policy with a specific list of redactions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | An array of redactions for the policy |

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Gets an array of fully configured  Redaction -derived classes.

**Returns:**
com.groupdocs.redaction.Redaction[] - An array of fully configured  Redaction -derived classes.
### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Loads an instance of  RedactionPolicy  from a file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Path to XML file |

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy
### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Loads an instance of  RedactionPolicy  from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| input | java.io.InputStream | Stream containing XML configuration |

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy
### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Saves the redaction policy to a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Path to file. |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves the redaction policy to a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Target stream to save the policy |

