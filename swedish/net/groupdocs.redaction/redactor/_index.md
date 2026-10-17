---
title: "Redactor"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en huvudklass som styr dokumentredigeringsprocessen och möjliggör att öppna, redigera och spara dokument."
type: docs
weight: 820
url: /sv/net/groupdocs.redaction/redactor/
---
## Redactor class

Representerar huvudklassen som styr dokumentraderingsprocessen, vilket möjliggör att öppna, radera och spara dokument.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Initierar en ny instans av [`Redactor`](../redactor)-klassen med en ström. |
| [Redactor](redactor#constructor_3)(string) | Initierar en ny instans av [`Redactor`](../redactor)-klassen med en filsökväg. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Initierar en ny instans av [`Redactor`](../redactor)-klassen för ett lösenordsskyddat dokument med en ström. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Initierar en ny instans av klassen [`Redactor`](../redactor) för ett lösenordsskyddat dokument med dess sökväg. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Initierar en ny instans av klassen [`Redactor`](../redactor) för ett lösenordsskyddat dokument med ström och inställningar. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Initierar en ny instans av klassen [`Redactor`](../redactor) för ett lösenordsskyddat dokument med dess sökväg och inställningar. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Tillämpar en maskering på dokumentet. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Tillämpar en maskeringspolicy på dokumentet. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Tillämpar en uppsättning maskeringar på dokumentet. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Frigör resurser. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Genererar förhandsgranskningsbilder av specifika sidor i ett givet bildformat. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Hämtar den allmänna informationen om dokumentet – storlek, sidantal osv. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Sparar dokumentet till en fil med följande alternativ: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Sparar dokumentet till en fil. |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | Sparar dokumentet till den angivna strömmen. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Exempel

Följande exempel visar hur man tillämpar en enskild maskering på dokumentet.

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

Följande exempel visar hur man tillämpar en lista med maskeringar på dokumentet.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... andra maskeringar
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, om minst en maskering misslyckades
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

Följande exempel visar hur man tillämpar en redigeringspolicy på alla filer i en given inkommande mapp och sparar till en av de utgående mapparna – för framgångsrikt uppdaterade filer och för misslyckade.

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

Följande exempel visar hur man öppnar lösenordsskyddade dokument med LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Här kan vi använda dokumentinstansen för att utföra maskeringar
}
```

Följande exempel visar hur man sparar ett dokument med SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Dokumentredigering sker här
       // ...
    
       // Spara dokumentet med standardalternativ (konvertera sidor till bilder, spara som PDF)
       redactor.Save();
    
       // Spara dokumentet i originalformat och skriv över originalfilen
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Spara dokumentet till filen "*_Redacted.*" i originalformat
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Spara dokumentet till "*_AnyText.*" (t.ex. tidsstämpel istället för "AnyText") i filnamnet utan rasterisering
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Se även

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
