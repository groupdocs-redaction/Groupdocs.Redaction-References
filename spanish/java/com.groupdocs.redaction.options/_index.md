---
title: "com.groupdocs.redaction.options"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "El paquete proporciona clases de opciones de carga y guardado."
type: docs
weight: 15
url: /es/java/com.groupdocs.redaction.options/
---

El paquete proporciona clases de opciones de carga y guardado.



## Clases

| Clase | Descripción |
| --- | --- |
| [LoadOptions](../com.groupdocs.redaction.options/loadoptions) | Proporciona opciones que se usarán para abrir un archivo. |
| [PreviewOptions](../com.groupdocs.redaction.options/previewoptions) | Proporciona opciones para establecer requisitos y delegados de flujo para la generación de vistas previas. |
| [RasterizationOptions](../com.groupdocs.redaction.options/rasterizationoptions) | Proporciona opciones para convertir archivos a PDF. |
| [RedactorSettings](../com.groupdocs.redaction.options/redactorsettings) | Representa la configuración de redacción, permitiendo personalizar el proceso de redacción. |
| [SaveOptions](../com.groupdocs.redaction.options/saveoptions) | Proporciona opciones para cambiar el nombre del archivo de salida y/o convertir el documento a PDF basado en imágenes (rasterización). |
| [WordprocessingSaveOptions](../com.groupdocs.redaction.options/wordprocessingsaveoptions) | Opciones de guardado de procesamiento de texto. |

## Interfaces

| Interfaz | Descripción |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.redaction.options/icreatepagestream) | Proporciona un método que devuelve un flujo para escribir los datos de vista previa de la página. |
| [ILogger](../com.groupdocs.redaction.options/ilogger) | Define la interfaz de un registrador que puede usarse para registrar eventos y errores en el proceso de redacción. |
| [IReleasePageStream](../com.groupdocs.redaction.options/ireleasepagestream) | Representa un método que libera el flujo creado por el delegado CreatePageStream. |

## Enumeraciones

| Enum | Descripción |
| --- | --- |
| [AdvancedRasterizationOptions](../com.groupdocs.redaction.options/advancedrasterizationoptions) | Una enumeración para gestionar las opciones avanzadas de rasterización que se aplicarán. |
| [PdfComplianceLevel](../com.groupdocs.redaction.options/pdfcompliancelevel) | Representa una lista de niveles de cumplimiento PDF compatibles. |
| [PreviewFormats](../com.groupdocs.redaction.options/previewformats) | Representa los formatos de vista previa compatibles. |
| [WordProcessingComplianceLevel](../com.groupdocs.redaction.options/wordprocessingcompliancelevel) | Niveles de cumplimiento OOXML para documentos de procesamiento de texto. |
