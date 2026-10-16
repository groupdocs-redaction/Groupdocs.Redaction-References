---
title: "Applica"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Applica una redazione al documento."
type: docs
weight: 20
url: /it/net/groupdocs.redaction/redactor/apply/
---
## Apply(Redaction) {#apply}

Applica una redazione al documento.

```csharp
public RedactorChangeLog Apply(Redaction redaction)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| redaction | Redaction | Un'istanza di [`Redaction`](../../redaction) da applicare |

### Valore di ritorno

Successo o fallimento e messaggio di errore in questo caso

### Esempi

Il seguente esempio dimostra l'applicazione di una singola redazione al documento.

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

### Vedi anche

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(Redaction[]) {#apply_2}

Applica un insieme di redazioni al documento.

```csharp
public RedactorChangeLog Apply(Redaction[] redactions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| redazioni | Redaction[] | Un array di redazioni da applicare |

### Valore di ritorno

Successo o fallimento e messaggio di errore in questo caso

### Esempi

Il seguente esempio dimostra l'applicazione di un elenco di redazioni al documento.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... altre redazioni
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, se almeno una redazione è fallita
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

### Vedi anche

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(RedactionPolicy) {#apply_1}

Applica una politica di redazione al documento.

```csharp
public RedactorChangeLog Apply(RedactionPolicy policy)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| politica | RedactionPolicy | Policy di redazione |

### Valore di ritorno

Successo o fallimento e messaggio di errore in questo caso

### Esempi

Il seguente esempio dimostra come applicare una politica di redazione a tutti i file all'interno di una cartella di ingresso specificata e salvarli in una delle cartelle di uscita — per i file aggiornati con successo e per quelli falliti.

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

### Vedi anche

* class [RedactorChangeLog](../../redactorchangelog)
* class [RedactionPolicy](../../redactionpolicy)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
