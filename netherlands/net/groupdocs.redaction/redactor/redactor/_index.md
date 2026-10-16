---
title: "Redactor"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Initialiseert een nieuwe instantie van de Redactorgroupdocs.redaction/redactor-klasse met behulp van het bestandspad."
type: docs
weight: 10
url: /nl/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Initialiseert een nieuwe instantie van de [`Redactor`](../../redactor)-klasse met behulp van het bestandspad.

```csharp
public Redactor(string filePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Pad naar het bestand |

### Voorbeelden

Het volgende voorbeeld toont hoe een document kan worden geopend voor redactie.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Hier kunnen we de documentinstantie gebruiken om redacties uit te voeren
}
```

### Zie ook

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Initialiseert een nieuwe instantie van de [`Redactor`](../../redactor)-klasse met behulp van een stream.

```csharp
public Redactor(Stream document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | Bronstream van het document |

### Voorbeelden

Het volgende voorbeeld toont hoe een document kan worden geopend vanuit een stream.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Hier kunnen we de documentinstantie gebruiken om redacties uit te voeren
    }
}
```

### Zie ook

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Initialiseert een nieuwe instantie van de [`Redactor`](../../redactor)-klasse voor een met wachtwoord beveiligd document met behulp van het pad.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Pad naar bestand. |
| loadOptions | LoadOptions | Opties, inclusief wachtwoord. |

### Zie ook

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Initialiseert een nieuwe instantie van de [`Redactor`](../../redactor)-klasse voor een met wachtwoord beveiligd document met behulp van het pad en de instellingen.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Pad naar bestand. |
| loadOptions | LoadOptions | Bestand-afhankelijke opties, inclusief wachtwoord. |
| instellingen | RedactorSettings | Standaardinstellingen voor het redactieproces. |

### Zie ook

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Initialiseert een nieuwe instantie van de [`Redactor`](../../redactor)-klasse voor een met wachtwoord beveiligd document met behulp van een stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | Bron-invoerstroom. |
| loadOptions | LoadOptions | Opties, inclusief wachtwoord. |

### Voorbeelden

Het volgende voorbeeld toont hoe een met wachtwoord beveiligd document te openen met LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier kunnen we de documentinstantie gebruiken om redacties uit te voeren
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Initialiseert een nieuw exemplaar van de klasse [`Redactor`](../../redactor) voor een met wachtwoord beveiligd document met behulp van een stream en instellingen.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | Bron-invoerstroom. |
| loadOptions | LoadOptions | Opties, inclusief wachtwoord. |
| instellingen | RedactorSettings | Standaardinstellingen voor het redactieproces. |

### Voorbeelden

Het volgende voorbeeld toont hoe een met wachtwoord beveiligd document te openen met LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier kunnen we de documentinstantie gebruiken om redacties uit te voeren
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
