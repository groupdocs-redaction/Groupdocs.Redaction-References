---
title: "ReplaceInColumn"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Vervangt alle overeenkomsten door een opgegeven vervanging in de gespecificeerde kolom en het werkblad."
type: docs
weight: 20
url: /nl/net/groupdocs.redaction.integration/icellularformatinstance/replaceincolumn/
---
## ReplaceInColumn(Regex, string, int, int) {#replaceincolumn_1}

Vervangt alle overeenkomsten door een opgegeven vervanging in de gespecificeerde kolom en het werkblad.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column, 
    int sheet)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| regularExpression | Regex | Reguliere expressie om te zoeken en te vervangen |
| vervanging | String | Tekstvervanging |
| kolom | Int32 | Kolomindex beginnend bij nul |
| werkblad | Int32 | Nul-gebaseerde werkbladindex |

### Retourwaarde

Vervangingsresultaat

### Zie ook

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

---

## ReplaceInColumn(Regex, string, int) {#replaceincolumn}

Vervangt alle overeenkomsten door een opgegeven vervanging in de gespecificeerde kolom op alle werkbladen.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| regularExpression | Regex | Reguliere expressie om te zoeken en te vervangen |
| vervanging | String | Tekstvervanging |
| kolom | Int32 | Kolomindex beginnend bij nul |

### Retourwaarde

Vervangingsresultaat

### Zie ook

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
