---
title: "groupdocs.redaction.integration"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Tipos bajo groupdocs.redaction.integration."
type: docs
url: /es/python-net/groupdocs.redaction.integration/
is_root: false
weight: 30
---


Tipos bajo `groupdocs.redaction.integration`.

### Clases
| Clase | Descripción |
| :- | :- |
| [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) | Representa un formato específico de un documento y puede implementarse para agregar tipos de documento personalizados. |
| [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/) | Define los métodos necesarios para acceder a anotaciones, como comentarios, y debe ser implementado por una clase derivada de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) para realizar redactados de anotaciones. |
| [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/) | Define los métodos necesarios para acceder a formatos de hojas de cálculo que contienen una o varias hojas de trabajo. |
| [`IFixedFormatDocument`](/redaction/python-net/groupdocs.redaction.integration/ifixedformatdocument/) | Define los métodos necesarios para acceder a formatos de estructura fija, como PDF o presentaciones. |
| [`IImageFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/iimageformatinstance/) | Define los métodos necesarios para redactar formatos de imágenes raster. |
| [`IMetadataAccess`](/redaction/python-net/groupdocs.redaction.integration/imetadataaccess/) | Define los métodos necesarios para acceder a los metadatos de un documento, si el formato lo admite. |
| [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/) | Define los métodos necesarios para manipular las páginas de un documento. Debe ser implementado por una clase derivada de [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) para realizar redactados de páginas. |
| [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/) | Define los métodos para crear una vista previa del documento. |
| [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/) | Define los métodos necesarios para guardar un documento en cualquier forma binaria. Los tipos incorporados guardan un documento como PDF con imágenes de sus páginas. |
| [`ITextualFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/itextualformatinstance/) | Representa una interfaz que define los métodos necesarios para redactar datos textuales en cualquier documento que contenga texto. |
| [`MetadataCollection`](/redaction/python-net/groupdocs.redaction.integration/metadatacollection/) | Representa un diccionario de [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) con su título como clave. |
| [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) | Representa un elemento de metadatos, común para todos los formatos compatibles y utilizado en redacciones de metadatos. |
