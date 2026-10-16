---
title: "Redactor"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een hoofdklasse voor die het documentredactieproces beheert, waardoor documenten geopend, geredigeerd en opgeslagen kunnen worden."
type: docs
weight: 820
url: /nl/net/groupdocs.redaction/redactor/
---
## Redactor class

Stelt een hoofdklasse voor die het documentredactietraject beheert, waardoor documenten kunnen worden geopend, geredigeerd en opgeslagen.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Initialiseert een nieuw exemplaar van de [`Redactor`](../redactor) klasse met behulp van een stream. |
| [Redactor](redactor#constructor_3)(string) | Initialiseert een nieuw exemplaar van de [`Redactor`](../redactor) klasse met behulp van een bestandspad. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Initialiseert een nieuw exemplaar van de [`Redactor`](../redactor) klasse voor een met wachtwoord beveiligd document met behulp van een stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Initialiseert een nieuw exemplaar van de [`Redactor`](../redactor) klasse voor een met wachtwoord beveiligd document met behulp van het pad. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Initialiseert een nieuw exemplaar van de [`Redactor`](../redactor) klasse voor een met wachtwoord beveiligd document met behulp van een stream en instellingen. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Initialiseert een nieuw exemplaar van de [`Redactor`](../redactor) klasse voor een met wachtwoord beveiligd document met behulp van het pad en instellingen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Past een redactie toe op het document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Past een redactieregel toe op het document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Past een reeks redacties toe op het document. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Vrijgeeft bronnen. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Genereert voorbeeldafbeeldingen van specifieke pagina's in een gegeven afbeeldingsformaat. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Haalt de algemene informatie over het document op - grootte, paginatelling, enz. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Slaat het document op in een bestand met de volgende opties: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Slaat het document op in een bestand. |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | Slaat het document op in de opgegeven stream. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Voorbeelden

Het volgende voorbeeld toont het toepassen van een enkele redactie op het document.

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

Het volgende voorbeeld toont het toepassen van een lijst met redacties op het document.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... andere redacties
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, als ten minste één redactie is mislukt
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

Het volgende voorbeeld toont hoe een redactiebeleid toe te passen op alle bestanden in een opgegeven inkomende map, en op te slaan in een van de uitgaande mappen - voor succesvol bijgewerkte bestanden en voor mislukte bestanden.

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

Het volgende voorbeeld toont hoe een met wachtwoord beveiligd document te openen met LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier kunnen we de documentinstantie gebruiken om redacties uit te voeren
}
```

Het volgende voorbeeld laat zien hoe een document op te slaan met SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Documentredactie komt hier
       // ...
    
       // Sla het document op met standaardopties (converteer pagina's naar afbeeldingen, sla op als PDF)
       redactor.Save();
    
       // Sla het document op in het oorspronkelijke formaat en overschrijf het originele bestand
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Sla het document op naar een \"*_Redacted.*\" bestand in het oorspronkelijke formaat
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Sla het document op naar \"*_AnyText.*\" (bijv. tijdstempel in plaats van \"AnyText\") in de bestandsnaam zonder rasterisatie
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Zie ook

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
