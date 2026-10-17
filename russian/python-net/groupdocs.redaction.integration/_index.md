---
title: "groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Типы в groupdocs.redaction.integration."
type: docs
url: /ru/python-net/groupdocs.redaction.integration/
is_root: false
weight: 30
---


Типы в `groupdocs.redaction.integration`.

### Классы
| Класс | Описание |
| :- | :- |
| [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) | Представляет конкретный формат документа и может быть реализован для добавления пользовательских типов документов. |
| [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/) | Определяет методы, необходимые для доступа к аннотациям, таким как комментарии, и должен быть реализован классом, производным от [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/), для выполнения редактирования аннотаций. |
| [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/) | Определяет методы, необходимые для доступа к форматам электронных таблиц, содержащим один или несколько листов. |
| [`IFixedFormatDocument`](/redaction/python-net/groupdocs.redaction.integration/ifixedformatdocument/) | Определяет методы, необходимые для доступа к форматам фиксированной структуры, таким как PDF или презентации. |
| [`IImageFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/iimageformatinstance/) | Определяет методы, необходимые для редактирования форматов растровых изображений. |
| [`IMetadataAccess`](/redaction/python-net/groupdocs.redaction.integration/imetadataaccess/) | Определяет методы, необходимые для доступа к метаданным документа, если формат их поддерживает. |
| [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/) | Определяет методы, необходимые для манипулирования страницами документа. Должен быть реализован классом, производным от [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/), для выполнения редактирования страниц. |
| [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/) | Определяет методы для создания предварительного просмотра документа. |
| [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/) | Определяет методы, необходимые для сохранения документа в любой бинарной форме. Встроенные типы сохраняют документ в виде PDF с изображениями его страниц. |
| [`ITextualFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/itextualformatinstance/) | Представляет интерфейс, определяющий методы, необходимые для редактирования текстовых данных в любом документе, содержащем текст. |
| [`MetadataCollection`](/redaction/python-net/groupdocs.redaction.integration/metadatacollection/) | Представляет словарь [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) с его заголовком в качестве ключа. |
| [`MetadataItem`](/redaction/python-net/groupdocs.redaction.integration/metadataitem/) | Представляет элемент метаданных, общий для всех поддерживаемых форматов и используемый в редактировании метаданных. |
