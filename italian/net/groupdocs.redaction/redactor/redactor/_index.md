---
title: "Redactor"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Inizializza una nuova istanza della classe Redactorgroupdocs.redaction/redactor utilizzando il percorso del file."
type: docs
weight: 10
url: /it/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Inizializza una nuova istanza della classe [`Redactor`](../../redactor) utilizzando il percorso del file.

```csharp
public Redactor(string filePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Percorso del file |

### Esempi

Il seguente esempio dimostra come aprire un documento per la redazione.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Qui possiamo usare l'istanza del documento per eseguire redazioni
}
```

### Vedi anche

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Inizializza una nuova istanza della classe [`Redactor`](../../redactor) utilizzando lo stream.

```csharp
public Redactor(Stream document)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| documento | Stream | Stream di origine del documento |

### Esempi

Il seguente esempio dimostra come aprire un documento dallo stream.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Qui possiamo usare l'istanza del documento per eseguire redazioni
    }
}
```

### Vedi anche

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Inizializza una nuova istanza della classe [`Redactor`](../../redactor) per un documento protetto da password utilizzando il suo percorso.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Percorso al file. |
| loadOptions | LoadOptions | Opzioni, inclusa la password. |

### Vedi anche

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Inizializza una nuova istanza della classe [`Redactor`](../../redactor) per un documento protetto da password utilizzando il suo percorso e le impostazioni.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Percorso al file. |
| loadOptions | LoadOptions | Opzioni dipendenti dal file, inclusa la password. |
| impostazioni | RedactorSettings | Impostazioni predefinite per il processo di redazione. |

### Vedi anche

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Inizializza una nuova istanza della classe [`Redactor`](../../redactor) per un documento protetto da password utilizzando lo stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| documento | Stream | Stream di input di origine. |
| loadOptions | LoadOptions | Opzioni, inclusa la password. |

### Esempi

Il seguente esempio dimostra come aprire documenti protetti da password usando LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Qui possiamo usare l'istanza del documento per eseguire redazioni
}
```

### Vedi anche

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Inizializza una nuova istanza della classe [`Redactor`](../../redactor) per un documento protetto da password usando lo stream e le impostazioni.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| documento | Stream | Stream di input di origine. |
| loadOptions | LoadOptions | Opzioni, inclusa la password. |
| impostazioni | RedactorSettings | Impostazioni predefinite per il processo di redazione. |

### Esempi

Il seguente esempio dimostra come aprire documenti protetti da password usando LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Qui possiamo usare l'istanza del documento per eseguire redazioni
}
```

### Vedi anche

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
