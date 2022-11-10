---
title: Redactor
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Initialise une nouvelle instance deRedactorgroupdocs.redaction/redactor classe utilisant le chemin du fichier.
type: docs
weight: 10
url: /fr/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Initialise une nouvelle instance de[`Redactor`](../../redactor) classe utilisant le chemin du fichier.

```csharp
public Redactor(string filePath)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Chemin d'accès au fichier |

### Exemples

L'exemple suivant montre comment ouvrir un document pour la rédaction.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Ici, nous pouvons utiliser une instance de document pour effectuer des suppressions
}
```

### Voir également

* class [Redactor](../../redactor)
* espace de noms [GroupDocs.Redaction](../../redactor)
* Assemblée [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Initialise une nouvelle instance de[`Redactor`](../../redactor) classe utilisant stream.

```csharp
public Redactor(Stream document)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| document | Stream | Flux source du document |

### Exemples

L'exemple suivant montre comment ouvrir un document à partir du flux.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Ici, nous pouvons utiliser une instance de document pour effectuer des suppressions
    }
}
```

### Voir également

* class [Redactor](../../redactor)
* espace de noms [GroupDocs.Redaction](../../redactor)
* Assemblée [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Initialise une nouvelle instance de[`Redactor`](../../redactor) classe pour un document protégé par mot de passe en utilisant son chemin.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Chemin d'accès au fichier. |
| loadOptions | LoadOptions | Options, y compris mot de passe. |

### Voir également

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* espace de noms [GroupDocs.Redaction](../../redactor)
* Assemblée [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Initialise une nouvelle instance de[`Redactor`](../../redactor) classe pour un document protégé par mot de passe en utilisant son chemin et ses paramètres.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Chemin d'accès au fichier. |
| loadOptions | LoadOptions | Options dépendantes du fichier, y compris le mot de passe. |
| settings | RedactorSettings | Paramètres par défaut pour le processus de rédaction. |

### Voir également

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* espace de noms [GroupDocs.Redaction](../../redactor)
* Assemblée [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Initialise une nouvelle instance de[`Redactor`](../../redactor) classe pour un document protégé par mot de passe utilisant stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| document | Stream | Flux d'entrée source. |
| loadOptions | LoadOptions | Options, y compris mot de passe. |

### Exemples

L'exemple suivant montre comment ouvrir un document protégé par mot de passe à l'aide de LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Ici, nous pouvons utiliser une instance de document pour effectuer des suppressions
}
```

### Voir également

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* espace de noms [GroupDocs.Redaction](../../redactor)
* Assemblée [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Initialise une nouvelle instance de[`Redactor`](../../redactor) classe pour un document protégé par mot de passe à l'aide du flux et des paramètres.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| document | Stream | Flux d'entrée source. |
| loadOptions | LoadOptions | Options, y compris mot de passe. |
| settings | RedactorSettings | Paramètres par défaut pour le processus de rédaction. |

### Exemples

L'exemple suivant montre comment ouvrir un document protégé par mot de passe à l'aide de LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Ici, nous pouvons utiliser une instance de document pour effectuer des suppressions
}
```

### Voir également

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* espace de noms [GroupDocs.Redaction](../../redactor)
* Assemblée [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
