---
title: "Redactor"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Initialise une nouvelle instance de la classe Redactorgroupdocs.redaction/redactor en utilisant le chemin du fichier."
type: docs
weight: 10
url: /fr/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Initialise une nouvelle instance de la classe [`Redactor`](../../redactor) en utilisant le chemin du fichier.

```csharp
public Redactor(string filePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | String | Chemin du fichier |

### Exemples

L'exemple suivant montre comment ouvrir un document pour la rédaction.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Ici nous pouvons utiliser l'instance du document pour effectuer des censures
}
```

### Voir aussi

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Initialise une nouvelle instance de la classe [`Redactor`](../../redactor) en utilisant le flux.

```csharp
public Redactor(Stream document)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Flux source du document |

### Exemples

L'exemple suivant montre comment ouvrir un document à partir du flux.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Ici nous pouvons utiliser l'instance du document pour effectuer des censures
    }
}
```

### Voir aussi

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Initialise une nouvelle instance de la classe [`Redactor`](../../redactor) pour un document protégé par mot de passe en utilisant son chemin.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | String | Chemin du fichier. |
| loadOptions | LoadOptions | Options, incluant le mot de passe. |

### Voir aussi

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Initialise une nouvelle instance de la classe [`Redactor`](../../redactor) pour un document protégé par mot de passe en utilisant son chemin et ses paramètres.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | String | Chemin du fichier. |
| loadOptions | LoadOptions | Options dépendant du fichier, incluant le mot de passe. |
| paramètres | RedactorSettings | Paramètres par défaut pour le processus de rédaction. |

### Voir aussi

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`Redactor`](../../redactor) pour un document protégé par mot de passe en utilisant le flux.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Flux d'entrée source. |
| loadOptions | LoadOptions | Options, incluant le mot de passe. |

### Exemples

L'exemple suivant montre comment ouvrir des documents protégés par mot de passe en utilisant LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Ici nous pouvons utiliser l'instance du document pour effectuer des censures
}
```

### Voir aussi

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Initialise une nouvelle instance de la classe [`Redactor`](../../redactor) pour un document protégé par mot de passe en utilisant un flux et des paramètres.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Flux d'entrée source. |
| loadOptions | LoadOptions | Options, incluant le mot de passe. |
| paramètres | RedactorSettings | Paramètres par défaut pour le processus de rédaction. |

### Exemples

L'exemple suivant montre comment ouvrir des documents protégés par mot de passe en utilisant LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Ici nous pouvons utiliser l'instance du document pour effectuer des censures
}
```

### Voir aussi

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
