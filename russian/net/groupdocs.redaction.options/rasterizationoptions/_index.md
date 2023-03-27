---
title: RasterizationOptions
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Предоставляет параметры для преобразования файлов в формат PDF.
type: docs
weight: 350
url: /ru/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Предоставляет параметры для преобразования файлов в формат PDF.

```csharp
public class RasterizationOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Инициализирует новый экземпляр. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Получает или задает уровень соответствия PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Получает или задает значение, указывающее, нужно ли все страницы документа преобразовать в изображения и поместить в один файл PDF. TRUE по умолчанию, установите FALSE, чтобы избежать растеризации. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Получает индикатор, который является истинным, если установлены расширенные параметры растеризации. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Получает или задает количество страниц, которые необходимо преобразовать в PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Получает или задает индекс первой страницы (на основе 0) для преобразования в PDF. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Этот метод можно использовать для регистрации расширенного параметра растеризации для применения. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Этот метод можно использовать для регистрации расширенного параметра растеризации для применения. |

### Примечания

**Узнать больше**

* Подробнее о сохранении документа в виде растрового PDF: [Сохранить в растрированном PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Подробнее о параметрах растеризации: [Выберите определенные страницы для растеризованного PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Примеры

В следующем примере показано, как установить параметры процесса растеризации.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // редактируем конфиденциальные данные на первом слайде 
    
        var rasterizationOptions = new RasterizationOptions();
        rasterizationOptions.PageIndex = 0;
        rasterizationOptions.PageCount = 1;
        rasterizationOptions.Compliance = PdfComplianceLevel.PdfA1a;
        using (var stream = File.Open(Path.Combine(@"C:\Temp", "PresentationFirstSlide.pdf")))
        {
            redactor.Save(stream, rasterizationOptions);
        }
    }      
```

В следующем примере показано, как применить расширенные параметры растеризации с настройками по умолчанию.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Сохраняем документ с параметрами по умолчанию (преобразование страниц в изображения, сохранение в формате PDF)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

В следующем примере показано, как применить параметр расширенной растеризации границ с пользовательскими настройками.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Сохраняем документ с пользовательской рамкой
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

В следующем примере показано, как применить параметр расширенной растеризации шума с пользовательскими настройками.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Сохраняем документ с произвольным количеством и размером шумовых эффектов
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

В следующем примере показано, как применить параметр расширенной растеризации наклона с пользовательскими настройками.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Сохраняем документ с пользовательским эффектом наклона
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Смотрите также

* пространство имен [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* сборка [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
