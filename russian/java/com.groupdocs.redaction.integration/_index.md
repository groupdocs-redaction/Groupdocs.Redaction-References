---
title: "com.groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Пакет предоставляет интерфейсы и классы, используемые для интеграции документов разных форматов с GroupDocs.Redactions."
type: docs
weight: 13
url: /ru/java/com.groupdocs.redaction.integration/
---

Пакет предоставляет интерфейсы и классы, используемые для интеграции документов разных форматов с GroupDocs.Redactions.



## Классы

| Класс | Описание |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | Представляет конкретный формат документа. |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | Представляет словарь объектов MetadataItem, где в качестве ключа используется его заголовок. |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | Представляет элемент метаданных, общий для всех поддерживаемых форматов и используемый при редактировании метаданных. |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | Представляет текст, извлечённый из изображения в результате процесса распознавания. |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | Предоставляет фасад для всех операций редактирования растровых изображений. |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | Представляет часть распознанного текста (слово, символ и т.д.), извлечённую OCR‑движком. |
| [TextLine](../com.groupdocs.redaction.integration/textline) | Представляет строку текста, извлечённую OCR‑движком из изображения. |

## Интерфейсы

| Интерфейс | Описание |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | Определяет методы, необходимые для доступа к аннотациям, таким как комментарии. |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | Определяет методы, необходимые для доступа к форматам электронных таблиц, содержащим один или несколько листов. |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | Определяет методы, необходимые для доступа к форматам фиксированной структуры, таким как PDF или презентации. |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | Определяет методы, необходимые для редактирования форматов растровых изображений. |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | Определяет методы, необходимые для доступа к метаданным документа, если формат их поддерживает. |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | Определяет методы, необходимые для одновременного редактирования нескольких областей изображения одним и тем же цветом. |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | Определяет методы, необходимые для применения текстовых редактирований к документам‑изображениям и вложенным изображениям. |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | Определяет методы, необходимые для управления страницами документа. |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | Определяет методы для создания предварительного просмотра документа. |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | Определяет методы, необходимые для сохранения документа в любой бинарной форме. |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | Определяет методы, необходимые для редактирования текстовых данных в любом документе, содержащем текст. |
