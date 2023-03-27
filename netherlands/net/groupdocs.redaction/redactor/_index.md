---
title: Redactor
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Vertegenwoordigt een hoofdklasse die het redactieproces van documenten bestuurt waardoor documenten kunnen worden geopend geredigeerd en opgeslagen.
type: docs
weight: 660
url: /nl/net/groupdocs.redaction/redactor/
---
## Redactor class

Vertegenwoordigt een hoofdklasse die het redactieproces van documenten bestuurt, waardoor documenten kunnen worden geopend, geredigeerd en opgeslagen.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Initialiseert een nieuw exemplaar van[`Redactor`](../redactor) klasse met behulp van stream. |
| [Redactor](redactor#constructor_3)(string) | Initialiseert een nieuw exemplaar van[`Redactor`](../redactor) klasse met bestandspad. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Initialiseert een nieuw exemplaar van[`Redactor`](../redactor) class voor een met een wachtwoord beveiligd document met behulp van stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Initialiseert een nieuw exemplaar van[`Redactor`](../redactor) klasse voor een met een wachtwoord beveiligd document met behulp van zijn path. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Initialiseert een nieuw exemplaar van[`Redactor`](../redactor)klasse voor een met een wachtwoord beveiligd document met behulp van stream en instellingen. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Initialiseert een nieuw exemplaar van[`Redactor`](../redactor) class voor een met een wachtwoord beveiligd document met behulp van het pad en de instellingen. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Past een redactie toe op het document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Past een redactiebeleid toe op het document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Past een reeks redacties toe op het document. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Geeft bronnen vrij. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Genereert voorbeeldafbeeldingen van specifieke pagina's in een bepaald afbeeldingsformaat. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Krijgt de algemene informatie over het document - grootte, aantal pagina's, etc. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Slaat het document op in een bestand met de volgende opties: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Slaat het document op in een bestand. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Slaat het document op in een stream, inclusief aangepaste locatie. |

### Opmerkingen

**Kom meer te weten**

* Meer informatie over het toepassen van redacties: [Basisprincipes van redactie](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Meer geavanceerde redactieonderwerpen: [Geavanceerd gebruik](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Voorbeelden

In het volgende voorbeeld ziet u hoe u een enkele redactie op het document toepast.

In het volgende voorbeeld ziet u hoe u een lijst met redacties toepast op het document.

Het volgende voorbeeld laat zien hoe u een redactiebeleid toepast op alle bestanden in een bepaalde inkomende map en opslaat in een van de uitgaande mappen - voor succesvol bijgewerkte bestanden en voor mislukte bestanden.

Het volgende voorbeeld laat zien hoe u met een wachtwoord beveiligde documenten kunt openen met behulp van LoadOptions.

Het volgende voorbeeld laat zien hoe u een document opslaat met SaveOptions.

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
    // Hier kunnen we documentinstanties gebruiken om redacties uit te voeren
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Documentredactie komt hier
       // ...
    
       // Sla het document op met standaardopties (pagina's converteren naar afbeeldingen, opslaan als PDF)
       redactor.Save();
    
       // Sla het document op in het originele formaat en overschrijf het originele bestand
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Sla het document op in het bestand "*_Redacted.*" in de originele indeling
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Sla het document op in "*_AnyText.*" (bijv. tijdstempel in plaats van "AnyText") in de bestandsnaam zonder rastering
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Zie ook

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* naamruimte [GroupDocs.Redaction](../../groupdocs.redaction)
* montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
