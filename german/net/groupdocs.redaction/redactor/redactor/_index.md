---
title: "Redactor"
second_title: "GroupDocs.Redaction für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der Redactorgroupdocs.redaction/redactor-Klasse mit Dateipfad."
type: docs
weight: 10
url: /de/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Initialisiert eine neue Instanz der [`Redactor`](../../redactor)-Klasse mit Dateipfad.

```csharp
public Redactor(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Pfad zur Datei |

### Beispiele

Das folgende Beispiel zeigt, wie man ein Dokument zur Redaktion öffnet.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Hier können wir die Dokumentinstanz verwenden, um Redaktionen durchzuführen
}
```

### Siehe auch

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Initialisiert eine neue Instanz der [`Redactor`](../../redactor)-Klasse mit Stream.

```csharp
public Redactor(Stream document)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dokument | Stream | Quell-Stream des Dokuments |

### Beispiele

Das folgende Beispiel zeigt, wie man ein Dokument aus einem Stream öffnet.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Hier können wir die Dokumentinstanz verwenden, um Redaktionen durchzuführen
    }
}
```

### Siehe auch

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Initialisiert eine neue Instanz der [`Redactor`](../../redactor)-Klasse für ein passwortgeschütztes Dokument mit dessen Pfad.

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
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Initialisiert eine neue Instanz der [`Redactor`](../../redactor)-Klasse für ein passwortgeschütztes Dokument mit dessen Pfad und Einstellungen.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Pfad zur Datei. |
| loadOptions | LoadOptions | Dateiabhängige Optionen, einschließlich Passwort. |
| Einstellungen | RedactorSettings | Standard-Einstellungen für den Redaktionsprozess. |

### Siehe auch

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`Redactor`](../../redactor)-Klasse für ein passwortgeschütztes Dokument mit Stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dokument | Stream | Quell-Eingabe-Stream. |
| loadOptions | LoadOptions | Optionen, einschließlich Passwort. |

### Beispiele

Das folgende Beispiel demonstriert, wie man passwortgeschützte Dokumente mit LoadOptions öffnet.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier können wir die Dokumentinstanz verwenden, um Redaktionen durchzuführen
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Initialisiert eine neue Instanz der [`Redactor`](../../redactor)-Klasse für ein passwortgeschütztes Dokument unter Verwendung von Stream und Einstellungen.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dokument | Stream | Quell-Eingabe-Stream. |
| loadOptions | LoadOptions | Optionen, einschließlich Passwort. |
| Einstellungen | RedactorSettings | Standard-Einstellungen für den Redaktionsprozess. |

### Beispiele

Das folgende Beispiel demonstriert, wie man passwortgeschützte Dokumente mit LoadOptions öffnet.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Hier können wir die Dokumentinstanz verwenden, um Redaktionen durchzuführen
}
```

### Siehe auch

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
