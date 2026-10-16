---
title: "com.groupdocs.redaction"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "El paquete proporciona clases para redactar información sensible de documentos en formatos PDF, imágenes raster y documentos de oficina."
type: docs
weight: 10
url: /es/java/com.groupdocs.redaction/
---

El paquete proporciona clases para redactar información sensible de documentos en formatos PDF, imágenes raster y documentos de oficina.

Las clases principales en este paquete son:

<br />

* [Redactor](../../com.groupdocs.redaction/redactor) is the entry point for redaction process.
* [Redaction](../../com.groupdocs.redaction/redaction) is abstract base class for all types of document redactions.
* [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) is pre-configured in XML set of redaction rules.
* [RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) provides information about redaction process results.

<br />




## Clases

| Clase | Descripción |
| --- | --- |
| [DocumentInfo](../com.groupdocs.redaction/documentinfo) | Representa información sobre el documento. |
| [FileType](../com.groupdocs.redaction/filetype) | Representa un tipo de archivo. |
| [PageInfo](../com.groupdocs.redaction/pageinfo) | Representa una breve información de página. |
| [Redaction](../com.groupdocs.redaction/redaction) | Representa una clase abstracta base para todos los tipos de redacción. |
| [RedactionPolicy](../com.groupdocs.redaction/redactionpolicy) | Representa una política de saneamiento, que contiene un conjunto de redacciones específicas a aplicar. |
| [RedactionResult](../com.groupdocs.redaction/redactionresult) | Representa un resultado de la operación de redacción. |
| [Redactor](../com.groupdocs.redaction/redactor) | Representa una clase principal que controla el proceso de redacción de documentos, permitiendo abrir, redactar y guardar documentos. |
| [RedactorChangeLog](../com.groupdocs.redaction/redactorchangelog) | Representa resultados para una lista de redacciones, pasados al método Apply() de la clase Redactor. |
| [RedactorLogEntry](../com.groupdocs.redaction/redactorlogentry) | Representa resultados de la aplicación de la redacción. |

## Interfaces

| Interfaz | Descripción |
| --- | --- |
| [IDocumentInfo](../com.groupdocs.redaction/idocumentinfo) | Define métodos que son necesarios para obtener información básica del documento. |

## Enumeraciones

| Enum | Descripción |
| --- | --- |
| [RedactionStatus](../com.groupdocs.redaction/redactionstatus) | Representa un estado de finalización de la redacción. |
