---
title: "ReplaceInColumn"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Ersätter alla matchningar med en given ersättning i den angivna kolumnen och arbetsbladet."
type: docs
weight: 20
url: /sv/net/groupdocs.redaction.integration/icellularformatinstance/replaceincolumn/
---
## ReplaceInColumn(Regex, string, int, int) {#replaceincolumn_1}

Ersätter alla matchningar med en given ersättning i den angivna kolumnen och arbetsbladet.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column, 
    int sheet)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| regularExpression | Regex | Reguljärt uttryck för sökning och ersättning |
| ersättning | String | Textuell ersättning |
| kolumn | Int32 | Nollbaserat kolumnindex |
| blad | Int32 | Nollbaserat arbetsbladsindex |

### Returvärde

Ersättningsresultat

### Se även

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

---

## ReplaceInColumn(Regex, string, int) {#replaceincolumn}

Ersätter alla matchningar med en given ersättning i den angivna kolumnen på alla arbetsblad.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| regularExpression | Regex | Reguljärt uttryck för sökning och ersättning |
| ersättning | String | Textuell ersättning |
| kolumn | Int32 | Nollbaserat kolumnindex |

### Returvärde

Ersättningsresultat

### Se även

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
