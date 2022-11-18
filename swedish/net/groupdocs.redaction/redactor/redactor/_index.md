---
title: Redactor
second_title: GroupDocs.Redaction för .NET API-referens
description: Initierar en ny instans avRedactorgroupdocs.redaction/redactor klass med filsökväg.
type: docs
weight: 10
url: /sv/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Initierar en ny instans av[`Redactor`](../../redactor) klass med filsökväg.

```csharp
public Redactor(string filePath)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Sökväg till filen |

### Exempel

Följande exempel visar hur man öppnar ett dokument för redigering.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Här kan vi använda dokumentinstans för att utföra redaktioner
}
```

### Se även

* class [Redactor](../../redactor)
* namnutrymme [GroupDocs.Redaction](../../redactor)
* hopsättning [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Initierar en ny instans av[`Redactor`](../../redactor) klass med stream.

```csharp
public Redactor(Stream document)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| document | Stream | Källström för dokumentet |

### Exempel

Följande exempel visar hur man öppnar ett dokument från stream.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Här kan vi använda dokumentinstans för att utföra redaktioner
    }
}
```

### Se även

* class [Redactor](../../redactor)
* namnutrymme [GroupDocs.Redaction](../../redactor)
* hopsättning [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Initierar en ny instans av[`Redactor`](../../redactor) klass för ett lösenordsskyddat dokument som använder dess sökväg.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Sökväg till fil. |
| loadOptions | LoadOptions | Alternativ, inklusive lösenord. |

### Se även

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namnutrymme [GroupDocs.Redaction](../../redactor)
* hopsättning [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Initierar en ny instans av[`Redactor`](../../redactor) klass för ett lösenordsskyddat dokument med dess sökväg och inställningar.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Sökväg till fil. |
| loadOptions | LoadOptions | Filberoende alternativ, inklusive lösenord. |
| settings | RedactorSettings | Standardinställningar för redigeringsprocessen. |

### Se även

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namnutrymme [GroupDocs.Redaction](../../redactor)
* hopsättning [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Initierar en ny instans av[`Redactor`](../../redactor) klass för ett lösenordsskyddat dokument med stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| document | Stream | Källindataström. |
| loadOptions | LoadOptions | Alternativ, inklusive lösenord. |

### Exempel

Följande exempel visar hur du öppnar ett lösenordsskyddat dokument med LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Här kan vi använda dokumentinstans för att utföra redaktioner
}
```

### Se även

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namnutrymme [GroupDocs.Redaction](../../redactor)
* hopsättning [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Initierar en ny instans av[`Redactor`](../../redactor) klass för ett lösenordsskyddat dokument med ström och inställningar.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| document | Stream | Källindataström. |
| loadOptions | LoadOptions | Alternativ, inklusive lösenord. |
| settings | RedactorSettings | Standardinställningar för redigeringsprocessen. |

### Exempel

Följande exempel visar hur du öppnar ett lösenordsskyddat dokument med LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Här kan vi använda dokumentinstans för att utföra redaktioner
}
```

### Se även

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namnutrymme [GroupDocs.Redaction](../../redactor)
* hopsättning [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
