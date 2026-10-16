---
title: "Toepassen"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Past een redactie toe op het document."
type: docs
weight: 20
url: /nl/net/groupdocs.redaction/redactor/apply/
---
## Apply(Redaction) {#apply}

Past een redactie toe op het document.

```csharp
public RedactorChangeLog Apply(Redaction redaction)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| redaction | Redaction | Een instantie van [`Redaction`](../../redaction) om toe te passen |

### Retourwaarde

Succes of mislukking en foutmelding in dit geval

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

### Zie ook

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(Redaction[]) {#apply_2}

Past een reeks redacties toe op het document.

```csharp
public RedactorChangeLog Apply(Redaction[] redactions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| redacties | Redaction[] | Een array van redactionele acties om toe te passen |

### Retourwaarde

Succes of mislukking en foutmelding in dit geval

### Voorbeelden

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

### Zie ook

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(RedactionPolicy) {#apply_1}

Past een redactieregel toe op het document.

```csharp
public RedactorChangeLog Apply(RedactionPolicy policy)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| beleid | RedactionPolicy | Redaction beleid |

### Retourwaarde

Succes of mislukking en foutmelding in dit geval

### Voorbeelden

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

### Zie ook

* class [RedactorChangeLog](../../redactorchangelog)
* class [RedactionPolicy](../../redactionpolicy)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
