---
title: Redactor
second_title: GroupDocs.Redaction für .NET-API-Referenz
description: Initialisiert eine neue Instanz vonRedactorgroupdocs.redaction/redactor Klasse mit Dateipfad.
type: docs
weight: 10
url: /de/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Initialisiert eine neue Instanz von[`Redactor`](../../redactor) Klasse mit Dateipfad.

```csharp
public Redactor(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Pfad zur Datei |

### Beispiele

Das folgende Beispiel zeigt, wie ein Dokument zum Schwärzen geöffnet wird.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Hier können wir die Dokumentinstanz verwenden, um Schwärzungen durchzuführen
}
```

### Siehe auch

* class [Redactor](../../redactor)
* namensraum [GroupDocs.Redaction](../../redactor)
* Montage [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Initialisiert eine neue Instanz von[`Redactor`](../../redactor) Klasse mit stream.

```csharp
public Redactor(Stream document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| document | Stream | Quellstream des Dokuments |

### Beispiele

Das folgende Beispiel zeigt, wie ein Dokument aus dem Stream geöffnet wird.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Hier können wir die Dokumentinstanz verwenden, um Schwärzungen durchzuführen
    }
}
```

### Siehe auch

* class [Redactor](../../redactor)
* namensraum [GroupDocs.Redaction](../../redactor)
* Montage [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Initialisiert eine neue Instanz von[`Redactor`](../../redactor) Klasse für ein passwortgeschütztes Dokument mit seinem Pfad.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Pfad zur Datei. |
| loadOptions | LoadOptions | Optionen, einschließlich Passwort. |

### Siehe auch

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namensraum [GroupDocs.Redaction](../../redactor)
* Montage [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Initialisiert eine neue Instanz von[`Redactor`](../../redactor) Klasse für ein passwortgeschütztes Dokument mit seinem Pfad und seinen Einstellungen.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Pfad zur Datei. |
| loadOptions | LoadOptions | Dateiabhängige Optionen, einschließlich Passwort. |
| settings | RedactorSettings | Standardeinstellungen für den Redaktionsprozess. |

### Siehe auch

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namensraum [GroupDocs.Redaction](../../redactor)
* Montage [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Initialisiert eine neue Instanz von[`Redactor`](../../redactor) Klasse für ein passwortgeschütztes Dokument mit stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| document | Stream | Quelleingangsstrom. |
| loadOptions | LoadOptions | Optionen, einschließlich Passwort. |

### Beispiele

Das folgende Beispiel zeigt, wie ein kennwortgeschütztes Dokument mit LoadOptions geöffnet wird.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier können wir die Dokumentinstanz verwenden, um Schwärzungen durchzuführen
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namensraum [GroupDocs.Redaction](../../redactor)
* Montage [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Initialisiert eine neue Instanz von[`Redactor`](../../redactor) Klasse für ein passwortgeschütztes Dokument mit Stream und Einstellungen.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| document | Stream | Quelleingangsstrom. |
| loadOptions | LoadOptions | Optionen, einschließlich Passwort. |
| settings | RedactorSettings | Standardeinstellungen für den Redaktionsprozess. |

### Beispiele

Das folgende Beispiel zeigt, wie ein kennwortgeschütztes Dokument mit LoadOptions geöffnet wird.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier können wir die Dokumentinstanz verwenden, um Schwärzungen durchzuführen
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namensraum [GroupDocs.Redaction](../../redactor)
* Montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
