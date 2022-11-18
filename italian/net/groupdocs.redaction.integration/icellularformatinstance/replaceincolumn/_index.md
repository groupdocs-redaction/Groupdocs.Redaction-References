---
title: ReplaceInColumn
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Sostituisce tutte le corrispondenze con una determinata sostituzione nella colonna e nel foglio di lavoro specificati.
type: docs
weight: 20
url: /it/net/groupdocs.redaction.integration/icellularformatinstance/replaceincolumn/
---
## ReplaceInColumn(Regex, string, int, int) {#replaceincolumn_1}

Sostituisce tutte le corrispondenze con una determinata sostituzione nella colonna e nel foglio di lavoro specificati.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column, 
    int sheet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| regularExpression | Regex | Espressione regolare da cercare e sostituire |
| replacement | String | Sostituzione testuale |
| column | Int32 | Indice di colonna in base zero |
| sheet | Int32 | Indice del foglio di lavoro in base zero |

### Valore di ritorno

Risultato sostituzione

### Guarda anche

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* spazio dei nomi [GroupDocs.Redaction.Integration](../../icellularformatinstance)
* assemblea [GroupDocs.Redaction](../../../)

---

## ReplaceInColumn(Regex, string, int) {#replaceincolumn}

Sostituisce tutte le corrispondenze con una data sostituzione nella colonna specificata su tutti i fogli di lavoro.

```csharp
public RedactionResult ReplaceInColumn(Regex regularExpression, string replacement, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| regularExpression | Regex | Espressione regolare da cercare e sostituire |
| replacement | String | Sostituzione testuale |
| column | Int32 | Indice di colonna in base zero |

### Valore di ritorno

Risultato sostituzione

### Guarda anche

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* interface [ICellularFormatInstance](../../icellularformatinstance)
* spazio dei nomi [GroupDocs.Redaction.Integration](../../icellularformatinstance)
* assemblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->