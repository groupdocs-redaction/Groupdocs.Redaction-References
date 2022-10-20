---
title: Initialize
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Выполняет инициализацию экземпляра обработчика формата документа.
type: docs
weight: 20
url: /ru/net/groupdocs.redaction.integration/documentformatinstance/initialize/
---
## DocumentFormatInstance.Initialize method

Выполняет инициализацию экземпляра обработчика формата документа.

```csharp
public virtual void Initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| config | DocumentFormatConfiguration | Конфигурация формата |
| settings | RedactorSettings | Настройки по умолчанию для процесса редактирования. |

### Примеры

В следующем примере показано, как использовать данные инициализации.

```csharp
public class MyCustomHandler : DocumentFormatInstance
{
    private string MyProperty { get; set; }
    
    // Другой пользовательский код 
    ...

    public override void Initialize(DocumentFormatConfiguration config)
    {
        base.Initialize(config);
        if (config.InitializationData.ContainsKey("MyProperty"))
        {
            MyProperty = config.InitializationData["MyProperty"];
        }
    }
}

// Подключаем пользовательский формат в GroupDocs.Redaction
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Смотрите также

* class [DocumentFormatConfiguration](../../../groupdocs.redaction.configuration/documentformatconfiguration)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [DocumentFormatInstance](../../documentformatinstance)
* пространство имен [GroupDocs.Redaction.Integration](../../documentformatinstance)
* сборка [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->