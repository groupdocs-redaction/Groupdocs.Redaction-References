---
title: "Redactor"
second_title: "GroupDocs.Redaction für .NET API-Referenz"
description: "Stellt die Hauptklasse dar, die den Dokumenten-Redaktionsprozess steuert und das Öffnen, Redigieren und Speichern von Dokumenten ermöglicht."
type: docs
weight: 820
url: /de/net/groupdocs.redaction/redactor/
---
## Redactor class

Stellt die Hauptklasse dar, die den Dokumenten-Redaktionsprozess steuert und das Öffnen, Redigieren und Speichern von Dokumenten ermöglicht.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Initialisiert eine neue Instanz der [`Redactor`](../redactor)-Klasse mithilfe eines Streams. |
| [Redactor](redactor#constructor_3)(string) | Initialisiert eine neue Instanz der [`Redactor`](../redactor)-Klasse mithilfe eines Dateipfads. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Initialisiert eine neue Instanz der [`Redactor`](../redactor)-Klasse für ein passwortgeschütztes Dokument mithilfe eines Streams. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Initialisiert eine neue Instanz der Klasse [`Redactor`](../redactor) für ein passwortgeschütztes Dokument unter Verwendung des Pfads. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Initialisiert eine neue Instanz der Klasse [`Redactor`](../redactor) für ein passwortgeschütztes Dokument unter Verwendung eines Streams und von Einstellungen. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Initialisiert eine neue Instanz der Klasse [`Redactor`](../redactor) für ein passwortgeschütztes Dokument unter Verwendung des Pfads und von Einstellungen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Wendet eine Redaktion auf das Dokument an. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Wendet eine Redaktionsrichtlinie auf das Dokument an. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Wendet eine Menge von Redaktionen auf das Dokument an. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Gibt Ressourcen frei. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Erzeugt Vorschaubilder bestimmter Seiten in einem angegebenen Bildformat. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Liefert die allgemeinen Informationen über das Dokument – Größe, Seitenanzahl usw. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Speichert das Dokument in einer Datei mit den folgenden Optionen: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Speichert das Dokument in einer Datei. |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | Speichert das Dokument in den angegebenen Stream. |

### Hinweise

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Beispiele

Das folgende Beispiel demonstriert das Anwenden einer einzelnen Redaktion auf das Dokument.

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

Das folgende Beispiel demonstriert das Anwenden einer Liste von Redaktionen auf das Dokument.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... andere Redaktionen
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, wenn mindestens eine Redaktion fehlgeschlagen ist
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

Das folgende Beispiel zeigt, wie man eine Redaktionsrichtlinie auf alle Dateien in einem angegebenen Eingangsordner anwendet und in einen der Ausgangsordner speichert – für erfolgreich aktualisierte Dateien und für fehlgeschlagene.

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

Das folgende Beispiel demonstriert, wie man passwortgeschützte Dokumente mit LoadOptions öffnet.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier können wir die Dokumentinstanz verwenden, um Redaktionen durchzuführen
}
```

Das folgende Beispiel zeigt, wie ein Dokument mit SaveOptions gespeichert wird.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Dokumenten-Redaktion kommt hier hin
       // ...
    
       // Dokument mit Standardoptionen speichern (Seiten in Bilder konvertieren, als PDF speichern)
       redactor.Save();
    
       // Dokument im Originalformat speichern und die Originaldatei überschreiben
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Dokument in eine "*_Redacted.*"-Datei im Originalformat speichern
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Dokument in "*_AnyText.*" (z. B. Zeitstempel anstelle von "AnyText") im Dateinamen speichern, ohne Rasterisierung
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Siehe auch

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
