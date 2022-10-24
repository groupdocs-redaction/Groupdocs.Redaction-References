---
title: com.groupdocs.redaction
second_title: GroupDocs.Redaction for Java API Reference
description: The package provides classes for redacting sensitive information from documents in PDF raster image and office document formats.
type: docs
weight: 10
url: /java/com.groupdocs.redaction/
---

The package provides classes for redacting sensitive information from documents in PDF, raster image and office document formats.

The main classes in this package are:

 *  [Redactor](../../com.groupdocs.redaction/redactor) is the entry point for redaction process.
 *  [Redaction](../../com.groupdocs.redaction/redaction) is abstract base class for all types of document redactions.
 *  [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) is pre-configured in XML set of redaction rules.
 *  [RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) provides information about redaction process results.


## Classes

| Class | Description |
| --- | --- |
| [DocumentInfo](../com.groupdocs.redaction/documentinfo) | Represents an information about document. |
| [FileType](../com.groupdocs.redaction/filetype) | Represents a file type. |
| [PageInfo](../com.groupdocs.redaction/pageinfo) | Represents a brief page information. |
| [Redaction](../com.groupdocs.redaction/redaction) | Represents a base abstract class for all redaction types. |
| [RedactionPolicy](../com.groupdocs.redaction/redactionpolicy) | Represents a sanitization policy, containing a set of specific redactions to apply. |
| [RedactionResult](../com.groupdocs.redaction/redactionresult) | Represents a result of the redaction operation. |
| [Redactor](../com.groupdocs.redaction/redactor) | Represents a main class that controls document redaction process, allowing to open, redact and save documents. |
| [RedactorChangeLog](../com.groupdocs.redaction/redactorchangelog) | Represents results for a list of redactions, passed to Apply() method of  Redactor  class. |
| [RedactorLogEntry](../com.groupdocs.redaction/redactorlogentry) | Represents results of applying redaction. |

## Interfaces

| Interface | Description |
| --- | --- |
| [IDocumentInfo](../com.groupdocs.redaction/idocumentinfo) | Defines methods that are required for getting basic document information. |

## Enumerations

| Enum | Description |
| --- | --- |
| [RedactionStatus](../com.groupdocs.redaction/redactionstatus) | Represents a redaction completion status. |
