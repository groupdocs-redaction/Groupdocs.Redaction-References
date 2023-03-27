---
title: AddAdvancedOption
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Этот метод можно использовать для регистрации расширенного параметра растеризации для применения.
type: docs
weight: 70
url: /ru/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Этот метод можно использовать для регистрации расширенного параметра растеризации для применения.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Предоставляет информацию о выбранном типе эффекта (оттенки серого, граница и т. д.) |

### Примеры

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

### Смотрите также

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* пространство имен [GroupDocs.Redaction.Options](../../rasterizationoptions)
* сборка [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Этот метод можно использовать для регистрации расширенного параметра растеризации для применения.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Предоставляет информацию о выбранном типе эффекта (оттенки серого, граница и т. д.) |
| parameters | Dictionary`2 | Параметры данного эффекта, такие как угол поворота |

### Примеры

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* пространство имен [GroupDocs.Redaction.Options](../../rasterizationoptions)
* сборка [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
