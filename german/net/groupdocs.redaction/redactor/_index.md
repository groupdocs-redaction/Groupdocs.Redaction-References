---
title: Redactor
second_title: GroupDocs.Redaction für .NET-API-Referenz
description: Stellt eine Hauptklasse dar die den Dokumentenschwärzungsprozess steuert und das Öffnen Schwärzen und Speichern von Dokumenten ermöglicht.
type: docs
weight: 650
url: /de/net/groupdocs.redaction/redactor/
---
## Redactor class

Stellt eine Hauptklasse dar, die den Dokumentenschwärzungsprozess steuert und das Öffnen, Schwärzen und Speichern von Dokumenten ermöglicht.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Initialisiert eine neue Instanz von[`Redactor`](../redactor) Klasse mit stream. |
| [Redactor](redactor#constructor_3)(string) | Initialisiert eine neue Instanz von[`Redactor`](../redactor) Klasse mit Dateipfad. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Initialisiert eine neue Instanz von[`Redactor`](../redactor) Klasse für ein passwortgeschütztes Dokument mit stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Initialisiert eine neue Instanz von[`Redactor`](../redactor) Klasse für ein passwortgeschütztes Dokument mit seinem Pfad. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Initialisiert eine neue Instanz von[`Redactor`](../redactor) Klasse für ein passwortgeschütztes Dokument mit Stream und Einstellungen. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Initialisiert eine neue Instanz von[`Redactor`](../redactor) Klasse für ein passwortgeschütztes Dokument mit seinem Pfad und seinen Einstellungen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Wendet eine Schwärzung auf das Dokument an. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Wendet eine Schwärzungsrichtlinie auf das Dokument an. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Wendet eine Reihe von Schwärzungen auf das Dokument an. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Gibt Ressourcen frei. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Erzeugt Vorschaubilder bestimmter Seiten in einem bestimmten Bildformat. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Ruft die allgemeinen Informationen über das Dokument ab – Größe, Seitenzahl usw. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Speichert das Dokument in einer Datei mit den folgenden Optionen: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Speichert das Dokument in einer Datei. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Speichert das Dokument in einem Stream, einschließlich benutzerdefiniertem Speicherort. |

### Bemerkungen

**Mehr erfahren**

* Weitere Details zum Anwenden von Schwärzungen: [Grundlagen der Redaktion](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Weiterführende Schwärzungsthemen: [Erweiterte Nutzung](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Beispiele

Das folgende Beispiel zeigt das Anwenden einer einzelnen Schwärzung auf das Dokument.

Das folgende Beispiel zeigt das Anwenden einer Schwärzungsliste auf das Dokument.

Das folgende Beispiel zeigt, wie eine Schwärzungsrichtlinie auf alle Dateien in einem bestimmten Eingangsordner angewendet und in einem der Ausgangsordner gespeichert wird – für erfolgreich aktualisierte Dateien und für fehlgeschlagene Dateien.

Das folgende Beispiel zeigt, wie ein kennwortgeschütztes Dokument mit LoadOptions geöffnet wird.

Das folgende Beispiel zeigt, wie ein Dokument mit SaveOptions gespeichert wird.

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
      // ... andere Schwärzungen
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // false, wenn mindestens eine Schwärzung fehlgeschlagen ist
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
    // Hier können wir die Dokumentinstanz verwenden, um Schwärzungen durchzuführen
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Das Schwärzen von Dokumenten gehört hierher
       // ...
    
       // Dokument mit Standardoptionen speichern (Seiten in Bilder umwandeln, als PDF speichern)
       redactor.Save();
    
       // Speichern Sie das Dokument im Originalformat und überschreiben Sie die Originaldatei
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Speichern Sie das Dokument im Originalformat in der Datei "*_Redacted.*".
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Speichern Sie das Dokument unter "*_AnyText.*" (z. B. Zeitstempel statt "AnyText") in seinem Dateinamen ohne Rasterung
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Siehe auch

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namensraum [GroupDocs.Redaction](../../groupdocs.redaction)
* Montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
