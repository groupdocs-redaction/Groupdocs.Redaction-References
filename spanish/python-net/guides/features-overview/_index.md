---
title: "Resumen de funciones"
linkTitle: "Features overview"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "GroupDocs.Redaction para Python a través de .NET elimina información sensible de los documentos mediante una única API independiente del formato — texto, metadatos, áreas de imagen, anotaciones y páginas completas — y guarda el resultado en el formato original o como un PDF sanitizado."
type: docs
url: /es/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction para Python a través de .NET elimina u oculta permanentemente información sensible en una amplia gama de [supported document formats](). Cada redacción sigue el mismo flujo de trabajo: abre un documento con [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/), aplica una o más redacciones con `apply()`, luego `save()` el resultado limpio ya sea en su formato original o como un PDF sanitizado. Las capacidades a continuación pueden combinarse libremente en una sola pasada.

## Text redaction

Buscar y reemplazar texto mediante una frase exacta o una expresión regular, abarcando tanto palabras completas como patrones complejos como direcciones de correo electrónico, números de teléfono o números de identificación nacional. El texto coincidente puede ser reemplazado por texto sustituto o cubierto por un cuadro coloreado para que el contenido original no pueda recuperarse. En hojas de cálculo puedes limitar la búsqueda a una sola hoja de trabajo o columna. Ver [Text Redactions]().

## Metadata redaction

Borrar o reescribir los metadatos del documento — autor, título, empresa, comentarios y datos EXIF en imágenes — para que no se filtren detalles sensibles a través de las propiedades del documento. Puedes eliminar todos los metadatos, apuntar a campos específicos o reemplazar valores por nuevos. Ver [Metadata Redactions]().

## Image-area redaction

Oscurecer una región rectangular de una imagen incrustada o de una página escaneada dibujando un cuadro relleno sobre el área dada — útil para ocultar firmas, fotos, encabezados o pies de página donde se espera que aparezcan datos confidenciales. Ver [Image Redactions]().

## Annotation redaction

Reescribir o eliminar anotaciones, comentarios y notas. Puedes quitar todas las anotaciones o usar una expresión regular para coincidir solo con aquellas que contengan texto sensible. Ver [Annotation Redactions]().

## Page removal

Eliminar páginas completas de documentos PDF, diapositivas de presentaciones y hojas de cálculo de libros de cálculo. Especificas una página inicial y una cantidad, junto con la dirección relativa al punto de inicio. Ver [Remove Page Redactions]().

## Rasterization to PDF

Guardar el documento limpiado como un PDF cuyas páginas se renderizan como imágenes rasterizadas. El archivo resultante no contiene texto buscable y no incluye los metadatos originales, por lo que el contenido eliminado no puede recuperarse. La rasterización es la opción adecuada cuando debes entregar un documento a terceros o cumplir con regulaciones que exigen PDF. Puedes seleccionar páginas específicas y solicitar cumplimiento PDF/A mediante las opciones avanzadas de rasterización. Ver [Save in Rasterized PDF]() y [Advanced Rasterization Options]().

## Redaction policies

Agrupar varias redacciones en una política reutilizable y aplicar el mismo conjunto de reglas de forma consistente en muchos documentos — ideal para tareas recurrentes como limpiar un conjunto estándar de campos antes de publicar. Ver [Use Redaction Policies]().

## Loading and saving

Cargar documentos desde una ruta local o desde un flujo, incluidos archivos protegidos con contraseña, y opcionalmente pre-rasterizar un documento antes de la redacción. Al guardar, conservar el formato original para edición posterior, sobrescribir el archivo original, rasterizar a PDF o escribir a un flujo. Ver [Loading Documents]() y [Saving Documents]().

## On-premise

GroupDocs.Redaction para Python vía .NET se ejecuta completamente en tu propia infraestructura — tus documentos nunca abandonan tu entorno. El paquete es una rueda autocontenida que incluye todo lo necesario, por lo que no es necesario instalar Microsoft Office, OpenOffice, Adobe Acrobat o un runtime separado. Ver [System Requirements]() para las plataformas compatibles y dependencias nativas.
