---
title: "ReplaceInColumn"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Sostituisce tutte le corrispondenze con una data sostituzione nella colonna e foglio di lavoro specificati."
type: docs
weight: 20
url: /it/net/groupdocs.redaction.integration/icellularformatinstance/replaceincolumn/
---
## ReplaceInColumn(Regex, string, int, int) {#replaceincolumn_1}

Sostituisce tutte le corrispondenze con una data sostituzione nella colonna e foglio di lavoro specificati.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column, 
    int sheet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| regularExpression | Regex | Espressione regolare per cercare e sostituire |
| sostituzione | String | Sostituzione testuale |
| colonna | Int32 | Indice della colonna a base zero |
| foglio | Int32 | Indice del foglio di lavoro basato su zero |

### Valore di ritorno

Risultato della sostituzione

### Vedi anche

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

---

## ReplaceInColumn(Regex, string, int) {#replaceincolumn}

Sostituisce tutte le corrispondenze con una data sostituzione nella colonna specificata su tutti i fogli di lavoro.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| regularExpression | Regex | Espressione regolare per cercare e sostituire |
| sostituzione | String | Sostituzione testuale |
| colonna | Int32 | Indice della colonna a base zero |

### Valore di ritorno

Risultato della sostituzione

### Vedi anche

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
