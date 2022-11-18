---
title: Redactor
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Inizializza una nuova istanza diRedactorgroupdocs.redaction/redactor classe utilizzando il percorso del file.
type: docs
weight: 10
url: /it/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Inizializza una nuova istanza di[`Redactor`](../../redactor) classe utilizzando il percorso del file.

```csharp
public Redactor(string filePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Percorso del file |

### Esempi

L'esempio seguente mostra come aprire un documento per la redazione.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Qui possiamo usare l'istanza del documento per eseguire redazioni
}
```

### Guarda anche

* class [Redactor](../../redactor)
* spazio dei nomi [GroupDocs.Redaction](../../redactor)
* assemblea [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Inizializza una nuova istanza di[`Redactor`](../../redactor) classe utilizzando stream.

```csharp
public Redactor(Stream document)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| document | Stream | Flusso di origine del documento |

### Esempi

L'esempio seguente mostra come aprire un documento dallo stream.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Qui possiamo usare l'istanza del documento per eseguire redazioni
    }
}
```

### Guarda anche

* class [Redactor](../../redactor)
* spazio dei nomi [GroupDocs.Redaction](../../redactor)
* assemblea [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Inizializza una nuova istanza di[`Redactor`](../../redactor) class per un documento protetto da password utilizzando il suo percorso.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Percorso al file. |
| loadOptions | LoadOptions | Opzioni, compresa la password. |

### Guarda anche

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* spazio dei nomi [GroupDocs.Redaction](../../redactor)
* assemblea [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Inizializza una nuova istanza di[`Redactor`](../../redactor) class per un documento protetto da password utilizzando il percorso e le impostazioni.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Percorso al file. |
| loadOptions | LoadOptions | Opzioni dipendenti dal file, inclusa la password. |
| settings | RedactorSettings | Impostazioni predefinite per il processo di redazione. |

### Guarda anche

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* spazio dei nomi [GroupDocs.Redaction](../../redactor)
* assemblea [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Inizializza una nuova istanza di[`Redactor`](../../redactor) class per un documento protetto da password utilizzando stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| document | Stream | Flusso di input di origine. |
| loadOptions | LoadOptions | Opzioni, compresa la password. |

### Esempi

L'esempio seguente mostra come aprire un documento protetto da password utilizzando LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Qui possiamo usare l'istanza del documento per eseguire redazioni
}
```

### Guarda anche

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* spazio dei nomi [GroupDocs.Redaction](../../redactor)
* assemblea [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Inizializza una nuova istanza di[`Redactor`](../../redactor) class per un documento protetto da password utilizzando stream e impostazioni.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| document | Stream | Flusso di input di origine. |
| loadOptions | LoadOptions | Opzioni, compresa la password. |
| settings | RedactorSettings | Impostazioni predefinite per il processo di redazione. |

### Esempi

L'esempio seguente mostra come aprire un documento protetto da password utilizzando LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Qui possiamo usare l'istanza del documento per eseguire redazioni
}
```

### Guarda anche

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* spazio dei nomi [GroupDocs.Redaction](../../redactor)
* assemblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
