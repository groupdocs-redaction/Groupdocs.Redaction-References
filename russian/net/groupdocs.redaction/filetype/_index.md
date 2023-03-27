---
title: FileType
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Представляет тип файла. Предоставляет методы для получения списка всех типов файлов поддерживаемых GroupDocs.Redaction определения типа файла по расширению и т. д.
type: docs
weight: 90
url: /ru/net/groupdocs.redaction/filetype/
---
## FileType class

Представляет тип файла. Предоставляет методы для получения списка всех типов файлов, поддерживаемых GroupDocs.Redaction, определения типа файла по расширению и т. д.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Файл растрового изображения (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Файл значений, разделенных запятыми (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Документ Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Документ Word Open XML с поддержкой макросов (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Документ Microsoft Word Open XML (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Шаблон документа Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Шаблон документа Word Open XML с поддержкой макросов (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Шаблон документа Word Open XML (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Графический файл формата обмена (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Файл языка разметки гипертекста (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Файл языка разметки гипертекста (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | Основной файл изображения JPEG 2000 (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Изображение JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Изображение JPEG (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Файл документации Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Электронная таблица номеров Apple (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Презентация OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | Электронная таблица OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | Текстовый документ OpenDocument (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Шаблон электронной таблицы OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Шаблон документа OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Файл переносимого формата документа (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Портативная сетевая графика (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Презентация PowerPoint (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | Презентация PowerPoint Open XML (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Файл в формате RTF (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Файл изображения с тегами (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Формат файла изображения с тегами (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Файл значений, разделенных табуляцией (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Простой текстовый файл (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Представляет неизвестный тип файла. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Электронная таблица Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Двоичная электронная таблица Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Электронная таблица Excel Open XML с поддержкой макросов (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Электронная таблица Microsoft Excel Open XML (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Получает суффикс имени файла (включая точку "."), например ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Получает имя типа файла, например "Документ Microsoft Word". |

## Методы

| Имя | Описание |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Сопоставляет расширение файла с типом файла. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Определяет, является ли текущий[`FileType`](../filetype) такое же, как указано[`FileType`](../filetype) объект. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Определяет, является ли текущий[`FileType`](../filetype) совпадает с указанным объектом. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Возвращает хеш-код для текущего[`FileType`](../filetype) объект. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Возвращает строку, представляющую текущий объект. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Извлекает поддерживаемые типы файлов |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Определяет, являются ли два[`FileType`](../filetype) объекты одинаковые. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Определяет, являются ли два[`FileType`](../filetype) объекты не одинаковы. |

### Примечания

**Узнать больше**

* [Поддерживаемые форматы документов](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Получить поддерживаемые форматы файлов](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Получить информацию о файле](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Смотрите также

* пространство имен [GroupDocs.Redaction](../../groupdocs.redaction)
* сборка [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
