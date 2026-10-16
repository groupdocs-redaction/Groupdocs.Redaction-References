---
title: "Appliquer"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Applique une censure au document."
type: docs
weight: 20
url: /fr/net/groupdocs.redaction/redactor/apply/
---
## Apply(Redaction) {#apply}

Applique une censure au document.

```csharp
public RedactorChangeLog Apply(Redaction redaction)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| redaction | Redaction | Une instance de [`Redaction`](../../redaction) à appliquer |

### Valeur de retour

Succès ou échec et message d'erreur dans ce cas

### Exemples

L'exemple suivant montre l'application d'une seule censure au document.

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

### Voir aussi

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(Redaction[]) {#apply_2}

Applique un ensemble de censures au document.

```csharp
public RedactorChangeLog Apply(Redaction[] redactions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rédactions | Redaction[] | Un tableau de redactions à appliquer |

### Valeur de retour

Succès ou échec et message d'erreur dans ce cas

### Exemples

L'exemple suivant montre l'application d'une liste de censures au document.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... autres censures
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, si au moins une censure a échoué
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

### Voir aussi

* class [RedactorChangeLog](../../redactorchangelog)
* class [Redaction](../../redaction)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Apply(RedactionPolicy) {#apply_1}

Applique une politique de censure au document.

```csharp
public RedactorChangeLog Apply(RedactionPolicy policy)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| politique | RedactionPolicy | Politique de rédaction |

### Valeur de retour

Succès ou échec et message d'erreur dans ce cas

### Exemples

L'exemple suivant montre comment appliquer une politique de rédaction à tous les fichiers d'un dossier d'entrée donné, et enregistrer dans l'un des dossiers de sortie – pour les fichiers mis à jour avec succès et pour ceux qui ont échoué.

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

### Voir aussi

* class [RedactorChangeLog](../../redactorchangelog)
* class [RedactionPolicy](../../redactionpolicy)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
