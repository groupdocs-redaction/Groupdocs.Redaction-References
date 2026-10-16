---
title: "com.groupdocs.redaction.integration"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "El paquete proporciona interfaces y clases utilizadas para integrar documentos de diferentes formatos con GroupDocs.Redactions."
type: docs
weight: 13
url: /es/java/com.groupdocs.redaction.integration/
---

El paquete proporciona interfaces y clases, utilizadas para integrar documentos de diferentes formatos con GroupDocs.Redactions.



## Clases

| Clase | Descripción |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | Representa un formato específico de un documento. |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | Representa un diccionario de MetadataItem con su título como clave. |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | Representa un elemento de metadatos, común para todos los formatos compatibles y usado en redactado de metadatos. |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | Representa texto, extraído de una imagen como resultado de su proceso de reconocimiento. |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | Proporciona una fachada para todas las operaciones de redacción de imágenes raster. |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | Representa una parte del texto reconocido (palabra, símbolo, etc.), extraído por el motor OCR. |
| [TextLine](../com.groupdocs.redaction.integration/textline) | Representa una línea de texto, extraída por el motor OCR de una imagen. |

## Interfaces

| Interfaz | Descripción |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | Define métodos que son necesarios para acceder a anotaciones, como comentarios. |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | Define métodos que son necesarios para acceder a formatos de hoja de cálculo, que tienen una o varias hojas de trabajo. |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | Define métodos que son necesarios para acceder a formatos de estructura fija, como PDF o presentaciones. |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | Define métodos que son necesarios para redactar formatos de imágenes raster. |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | Define métodos que son necesarios para acceder a los metadatos de un documento, si el formato lo admite. |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | Define métodos que son necesarios para redactar múltiples áreas de imagen a la vez con el mismo color. |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | Define métodos que son necesarios para aplicar redactados de texto a documentos de imagen e imágenes incrustadas. |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | Define métodos que son necesarios para manipular las páginas de un documento. |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | Define métodos para crear una vista previa del documento. |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | Define métodos que son necesarios para guardar el documento en cualquier forma binaria. |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | Define métodos que son necesarios para redactar datos de texto en cualquier documento que contenga texto. |
