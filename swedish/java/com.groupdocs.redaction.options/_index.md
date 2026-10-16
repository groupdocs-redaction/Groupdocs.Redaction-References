---
title: "com.groupdocs.redaction.options"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Paketet tillhandahåller klasser för inläsnings- och sparalternativ."
type: docs
weight: 15
url: /sv/java/com.groupdocs.redaction.options/
---

Paketet tillhandahåller klasser för inläsnings- och sparalternativ.



## Klasser

| Klass | Beskrivning |
| --- | --- |
| [LoadOptions](../com.groupdocs.redaction.options/loadoptions) | Tillhandahåller alternativ som kommer att användas för att öppna en fil. |
| [PreviewOptions](../com.groupdocs.redaction.options/previewoptions) | Tillhandahåller alternativ för att ange krav och strömdelegater för förhandsgranskningsgenerering. |
| [RasterizationOptions](../com.groupdocs.redaction.options/rasterizationoptions) | Tillhandahåller alternativ för att konvertera filer till PDF. |
| [RedactorSettings](../com.groupdocs.redaction.options/redactorsettings) | Representerar raderingsinställningar som möjliggör anpassning av raderingsprocessen. |
| [SaveOptions](../com.groupdocs.redaction.options/saveoptions) | Tillhandahåller alternativ för att ändra namn på utdatafilen och/eller konvertera dokumentet till bildbaserad PDF (rasterisering). |
| [WordprocessingSaveOptions](../com.groupdocs.redaction.options/wordprocessingsaveoptions) | Sparaalternativ för ordbehandling. |

## Gränssnitt

| Gränssnitt | Beskrivning |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.redaction.options/icreatepagestream) | Tillhandahåller en metod som returnerar en ström för att skriva förhandsgranskningsdata för sidan. |
| [ILogger](../com.groupdocs.redaction.options/ilogger) | Definierar gränssnittet för en logger som kan användas för att logga händelser och fel i raderingsprocessen. |
| [IReleasePageStream](../com.groupdocs.redaction.options/ireleasepagestream) | Representerar en metod som frigör strömmen som skapats av delegaten CreatePageStream. |

## Enumerationer

| Enum | Beskrivning |
| --- | --- |
| [AdvancedRasterizationOptions](../com.groupdocs.redaction.options/advancedrasterizationoptions) | En enumeration för att hantera de avancerade rasteriseringsalternativen som ska tillämpas. |
| [PdfComplianceLevel](../com.groupdocs.redaction.options/pdfcompliancelevel) | Representerar en lista över stödjade PDF-efterlevnadsnivåer. |
| [PreviewFormats](../com.groupdocs.redaction.options/previewformats) | Representerar stödjade förhandsgranskningsformat. |
| [WordProcessingComplianceLevel](../com.groupdocs.redaction.options/wordprocessingcompliancelevel) | OOXML-efterlevnadsnivåer för ordbehandlingsdokument. |
