---
title: DocumentFormatConfiguration
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Представляет ссылку на тип дляDocumentFormatInstance../groupdocs.redaction.integration/documentformatinstance Производный класс и список поддерживаемых расширений файлов для более быстрого определения формата.
type: docs
weight: 10
url: /ru/net/groupdocs.redaction.configuration/documentformatconfiguration/
---
## DocumentFormatConfiguration class

Представляет ссылку на тип для[`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) -Производный класс и список поддерживаемых расширений файлов для более быстрого определения формата.

```csharp
public class DocumentFormatConfiguration
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DocumentFormatConfiguration](documentformatconfiguration)() | Инициализирует новый экземпляр класса DocumentFormatConfiguration. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [DocumentType](../../groupdocs.redaction.configuration/documentformatconfiguration/documenttype) { get; set; } | Получает или задает тип класса, наследуя от[`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) . |
| [ExtensionFilter](../../groupdocs.redaction.configuration/documentformatconfiguration/extensionfilter) { get; set; } | Получает или задает разделенный запятыми (",") список расширений файлов (например, ".pdf") без учета регистра. |
| [InitializationData](../../groupdocs.redaction.configuration/documentformatconfiguration/initializationdata) { get; set; } | Получает или задает данные, необходимые для[`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) инициализация. |

## Методы

| Имя | Описание |
| --- | --- |
| [SupportsExtension](../../groupdocs.redaction.configuration/documentformatconfiguration/supportsextension)(string) | Проверяет, может ли данное расширение файла обрабатываться как DocumentType. |

### Примечания

**Узнать больше**

* Подробнее о**GroupDocs.Редактирование** конфигурация: [Расширить список поддерживаемых расширений](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* Подробнее о реализации пользовательских форматов: [Создать обработчик пользовательского формата](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Примеры

В следующем примере показано, как задать свойства для пользовательской конфигурации формата.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
```

### Смотрите также

* пространство имен [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* сборка [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
