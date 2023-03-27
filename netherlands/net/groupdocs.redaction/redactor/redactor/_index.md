---
title: Redactor
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Initialiseert een nieuw exemplaar vanRedactorgroupdocs.redaction/redactor klasse met bestandspad.
type: docs
weight: 10
url: /nl/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Initialiseert een nieuw exemplaar van[`Redactor`](../../redactor) klasse met bestandspad.

```csharp
public Redactor(string filePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Pad naar het bestand |

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een document opent voor redactie.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Hier kunnen we documentinstanties gebruiken om redacties uit te voeren
}
```

### Zie ook

* class [Redactor](../../redactor)
* naamruimte [GroupDocs.Redaction](../../redactor)
* montage [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Initialiseert een nieuw exemplaar van[`Redactor`](../../redactor) klasse met behulp van stream.

```csharp
public Redactor(Stream document)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | Bronstroom van het document |

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een document opent vanuit stream.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Hier kunnen we documentinstanties gebruiken om redacties uit te voeren
    }
}
```

### Zie ook

* class [Redactor](../../redactor)
* naamruimte [GroupDocs.Redaction](../../redactor)
* montage [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Initialiseert een nieuw exemplaar van[`Redactor`](../../redactor) klasse voor een met een wachtwoord beveiligd document met behulp van zijn path.

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
* naamruimte [GroupDocs.Redaction](../../redactor)
* montage [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Initialiseert een nieuw exemplaar van[`Redactor`](../../redactor) class voor een met een wachtwoord beveiligd document met behulp van het pad en de instellingen.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Pad naar bestand. |
| loadOptions | LoadOptions | Bestandsafhankelijke opties, inclusief wachtwoord. |
| settings | RedactorSettings | Standaardinstellingen voor redactieproces. |

### Zie ook

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* naamruimte [GroupDocs.Redaction](../../redactor)
* montage [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van[`Redactor`](../../redactor) class voor een met een wachtwoord beveiligd document met behulp van stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | Bron invoerstroom. |
| loadOptions | LoadOptions | Opties, inclusief wachtwoord. |

### Voorbeelden

Het volgende voorbeeld laat zien hoe u met een wachtwoord beveiligde documenten kunt openen met behulp van LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier kunnen we documentinstanties gebruiken om redacties uit te voeren
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* naamruimte [GroupDocs.Redaction](../../redactor)
* montage [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Initialiseert een nieuw exemplaar van[`Redactor`](../../redactor)klasse voor een met een wachtwoord beveiligd document met behulp van stream en instellingen.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | Bron invoerstroom. |
| loadOptions | LoadOptions | Opties, inclusief wachtwoord. |
| settings | RedactorSettings | Standaardinstellingen voor redactieproces. |

### Voorbeelden

Het volgende voorbeeld laat zien hoe u met een wachtwoord beveiligde documenten kunt openen met behulp van LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier kunnen we documentinstanties gebruiken om redacties uit te voeren
}
```

### Zie ook

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* naamruimte [GroupDocs.Redaction](../../redactor)
* montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
