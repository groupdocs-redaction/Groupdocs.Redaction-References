---
title: Redactor
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Инициализирует новый экземплярRedactorgroupdocs.redaction/redactor класс используя путь к файлу.
type: docs
weight: 10
url: /ru/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Инициализирует новый экземпляр[`Redactor`](../../redactor) класс, используя путь к файлу.

```csharp
public Redactor(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу |

### Примеры

В следующем примере показано, как открыть документ для редактирования.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Здесь мы можем использовать экземпляр документа для редактирования
}
```

### Смотрите также

* class [Redactor](../../redactor)
* пространство имен [GroupDocs.Redaction](../../redactor)
* сборка [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Инициализирует новый экземпляр[`Redactor`](../../redactor) класс, использующий stream.

```csharp
public Redactor(Stream document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| document | Stream | Исходный поток документа |

### Примеры

В следующем примере показано, как открыть документ из потока.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Здесь мы можем использовать экземпляр документа для редактирования
    }
}
```

### Смотрите также

* class [Redactor](../../redactor)
* пространство имен [GroupDocs.Redaction](../../redactor)
* сборка [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Инициализирует новый экземпляр[`Redactor`](../../redactor) класс для защищенного паролем документа, используя его путь.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |
| loadOptions | LoadOptions | Опции, включая пароль. |

### Смотрите также

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* пространство имен [GroupDocs.Redaction](../../redactor)
* сборка [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Инициализирует новый экземпляр[`Redactor`](../../redactor) class для защищенного паролем документа, используя его путь и настройки.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |
| loadOptions | LoadOptions | Параметры, зависящие от файла, включая пароль. |
| settings | RedactorSettings | Настройки по умолчанию для процесса редактирования. |

### Смотрите также

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* пространство имен [GroupDocs.Redaction](../../redactor)
* сборка [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Инициализирует новый экземпляр[`Redactor`](../../redactor) class для защищенного паролем документа с помощью stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| document | Stream | Исходный входной поток. |
| loadOptions | LoadOptions | Опции, включая пароль. |

### Примеры

В следующем примере показано, как открыть защищенный паролем документ с помощью LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Здесь мы можем использовать экземпляр документа для редактирования
}
```

### Смотрите также

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* пространство имен [GroupDocs.Redaction](../../redactor)
* сборка [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Инициализирует новый экземпляр[`Redactor`](../../redactor)класс для документа, защищенного паролем, с использованием потока и настроек.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| document | Stream | Исходный входной поток. |
| loadOptions | LoadOptions | Опции, включая пароль. |
| settings | RedactorSettings | Настройки по умолчанию для процесса редактирования. |

### Примеры

В следующем примере показано, как открыть защищенный паролем документ с помощью LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Здесь мы можем использовать экземпляр документа для редактирования
}
```

### Смотрите также

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* пространство имен [GroupDocs.Redaction](../../redactor)
* сборка [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
