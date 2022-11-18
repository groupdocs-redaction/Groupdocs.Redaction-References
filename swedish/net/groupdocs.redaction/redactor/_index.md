---
title: Redactor
second_title: GroupDocs.Redaction för .NET API-referens
description: Representerar en huvudklass som styr dokumentredigeringsprocessen vilket gör det möjligt att öppna redigera och spara dokument.
type: docs
weight: 650
url: /sv/net/groupdocs.redaction/redactor/
---
## Redactor class

Representerar en huvudklass som styr dokumentredigeringsprocessen, vilket gör det möjligt att öppna, redigera och spara dokument.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Initierar en ny instans av[`Redactor`](../redactor) klass med stream. |
| [Redactor](redactor#constructor_3)(string) | Initierar en ny instans av[`Redactor`](../redactor) klass med filsökväg. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Initierar en ny instans av[`Redactor`](../redactor) klass för ett lösenordsskyddat dokument med stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Initierar en ny instans av[`Redactor`](../redactor) klass för ett lösenordsskyddat dokument som använder dess sökväg. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Initierar en ny instans av[`Redactor`](../redactor) klass för ett lösenordsskyddat dokument med ström och inställningar. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Initierar en ny instans av[`Redactor`](../redactor) klass för ett lösenordsskyddat dokument med dess sökväg och inställningar. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Tillämpar en redigering på dokumentet. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Tillämpar en redigeringspolicy på dokumentet. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Tillämpar en uppsättning redigeringar på dokumentet. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Frigör resurser. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Genererar förhandsvisningsbilder av specifika sidor i ett givet bildformat. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Får allmän information om dokumentet - storlek, sidantal, etc. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Sparar dokumentet till en fil med följande alternativ: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Sparar dokumentet till en fil. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Sparar dokumentet i en ström, inklusive anpassad plats. |

### Anmärkningar

**Läs mer**

* Mer information om att tillämpa redigeringar: [Grundläggande om redigering](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Mer avancerade redigeringsämnen: [Avancerad användning](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Exempel

Följande exempel visar tillämpning av en enda redigering på dokumentet.

Följande exempel visar hur en lista med redigeringar tillämpas på dokumentet.

Följande exempel visar hur man tillämpar en redigeringspolicy på alla filer i en given inkommande mapp och sparar i en av utgående mappar - för framgångsrikt uppdaterade filer och för misslyckade.

Följande exempel visar hur du öppnar ett lösenordsskyddat dokument med LoadOptions.

Följande exempel visar hur man sparar ett dokument med Sparaalternativ.

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
      // ... andra redaktioner
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // false, om minst en redigering misslyckades
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
    // Här kan vi använda dokumentinstans för att utföra redaktioner
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Dokumentredigering går här
       // ...
    
       // Spara dokumentet med standardalternativ (konvertera sidor till bilder, spara som PDF)
       redactor.Save();
    
       // Spara dokumentet i originalformat och skriv över originalfilen
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Spara dokumentet till filen "*_Redacted.*" i originalformat
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Spara dokumentet till "*_AnyText.*" (t.ex. tidsstämpel istället för "AnyText") i dess filnamn utan rasterisering
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Se även

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namnutrymme [GroupDocs.Redaction](../../groupdocs.redaction)
* hopsättning [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
