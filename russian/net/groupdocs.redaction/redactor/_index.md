---
title: Redactor
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Представляет основной класс управляющий процессом редактирования документа позволяющий открывать редактировать и сохранять документы.
type: docs
weight: 650
url: /ru/net/groupdocs.redaction/redactor/
---
## Redactor class

Представляет основной класс, управляющий процессом редактирования документа, позволяющий открывать, редактировать и сохранять документы.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Инициализирует новый экземпляр[`Redactor`](../redactor) класс, использующий stream. |
| [Redactor](redactor#constructor_3)(string) | Инициализирует новый экземпляр[`Redactor`](../redactor) класс, используя путь к файлу. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Инициализирует новый экземпляр[`Redactor`](../redactor) class для защищенного паролем документа с помощью stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Инициализирует новый экземпляр[`Redactor`](../redactor) класс для защищенного паролем документа, используя его путь. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Инициализирует новый экземпляр[`Redactor`](../redactor) класс для документа, защищенного паролем, с использованием потока и настроек. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Инициализирует новый экземпляр[`Redactor`](../redactor) class для защищенного паролем документа, используя его путь и настройки. |

## Методы

| Имя | Описание |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Применяет редактирование к документу. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Применяет политику редактирования к документу. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Применяет набор исправлений к документу. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Освобождает ресурсы. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Генерирует изображения для предварительного просмотра определенных страниц в заданном формате изображения. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Получает общую информацию о документе - размер, количество страниц и т. д. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Сохраняет документ в файл со следующими параметрами: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Сохраняет документ в файл. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Сохраняет документ в поток, включая пользовательское местоположение. |

### Примечания

**Учить больше**

* Подробнее о применении правок: [Основы редактирования](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Дополнительные темы редактирования: [Расширенное использование](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Примеры

В следующем примере показано применение к документу единственного исправления.

В следующем примере показано применение списка исправлений к документу.

В следующем примере показано, как применить политику редактирования ко всем файлам в заданной входящей папке и сохранить в одной из исходящих папок — для успешно обновленных файлов и для неудачно обновленных.

В следующем примере показано, как открыть защищенный паролем документ с помощью LoadOptions.

В следующем примере показано, как сохранить документ с помощью SaveOptions.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... другие правки
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // false, если хотя бы одно редактирование не удалось
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Здесь мы можем использовать экземпляр документа для редактирования
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Здесь идет редактирование документа
       // ...
    
       // Сохраняем документ с параметрами по умолчанию (преобразование страниц в изображения, сохранение в формате PDF)
       redactor.Save();
    
       // Сохраняем документ в исходном формате, перезаписывая исходный файл
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Сохраняем документ в файл "*_Redacted.*" в оригинальном формате
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Сохраняем документ в "*_AnyText.*" (например, временная метка вместо "AnyText") в его имени файла без растеризации
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Смотрите также

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* пространство имен [GroupDocs.Redaction](../../groupdocs.redaction)
* сборка [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
