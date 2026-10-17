---
title: "Redactor"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Initierar en ny instans av Redactorgroupdocs.redaction/redactor-klass med filväg."
type: docs
weight: 10
url: /sv/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Initierar en ny instans av [`Redactor`](../../redactor)-klass med filväg.

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
    // Här kan vi använda dokumentinstansen för att utföra maskeringar
}
```

### Se även

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Initierar en ny instans av [`Redactor`](../../redactor)-klass med ström.

```csharp
public Redactor(Stream document)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dokument | Stream | Källströmmen för dokumentet |

### Exempel

Följande exempel visar hur man öppnar ett dokument från ström.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Här kan vi använda dokumentinstansen för att utföra maskeringar
    }
}
```

### Se även

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Initierar en ny instans av [`Redactor`](../../redactor)-klass för ett lösenordsskyddat dokument med dess sökväg.

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
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Initierar en ny instans av [`Redactor`](../../redactor)-klass för ett lösenordsskyddat dokument med dess sökväg och inställningar.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Sökväg till fil. |
| loadOptions | LoadOptions | Fil-beroende alternativ, inklusive lösenord. |
| settings | RedactorSettings | Standardinställningar för raderingsprocessen. |

### Se även

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Initierar en ny instans av [`Redactor`](../../redactor)-klass för ett lösenordsskyddat dokument med ström.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dokument | Stream | Källinmatningsström. |
| loadOptions | LoadOptions | Alternativ, inklusive lösenord. |

### Exempel

Följande exempel visar hur man öppnar lösenordsskyddade dokument med LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Här kan vi använda dokumentinstansen för att utföra maskeringar
}
```

### Se även

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Initierar en ny instans av [`Redactor`](../../redactor)-klassen för ett lösenordsskyddat dokument med hjälp av ström och inställningar.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dokument | Stream | Källinmatningsström. |
| loadOptions | LoadOptions | Alternativ, inklusive lösenord. |
| settings | RedactorSettings | Standardinställningar för raderingsprocessen. |

### Exempel

Följande exempel visar hur man öppnar lösenordsskyddade dokument med LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Här kan vi använda dokumentinstansen för att utföra maskeringar
}
```

### Se även

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
