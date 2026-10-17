---
title: "Verkställ"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tillämpar en maskering på dokumentet."
type: docs
weight: 20
url: /sv/net/groupdocs.redaction/redactor/apply/
---
## Apply(Redaction) {#apply}

Tillämpar en maskering på dokumentet.

```csharp
public RedactorChangeLog Apply(Redaction redaction)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| redaction | Redaction | En instans av [`Redaction`](../../redaction) att tillämpa |

### Returvärde

Framgång eller misslyckande och felmeddelande i detta fall

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

### Se även

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(Redaction[]) {#apply_2}

Tillämpar en uppsättning maskeringar på dokumentet.

```csharp
public RedactorChangeLog Apply(Redaction[] redactions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| raderingar | Redaction[] | En array av redactions att verkställa |

### Returvärde

Framgång eller misslyckande och felmeddelande i detta fall

### Exempel

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

### Se även

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(RedactionPolicy) {#apply_1}

Tillämpar en maskeringspolicy på dokumentet.

```csharp
public RedactorChangeLog Apply(RedactionPolicy policy)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| policy | RedactionPolicy | Raderingspolicy |

### Returvärde

Framgång eller misslyckande och felmeddelande i detta fall

### Exempel

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

### Se även

* class [RedactorChangeLog](../../redactorchangelog)
* class [RedactionPolicy](../../redactionpolicy)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
