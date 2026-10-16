---
title: "License"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Biedt methoden voor het toepassen van een licentie."
type: docs
weight: 270
url: /nl/net/groupdocs.redaction/license/
---
## License class

Biedt methoden voor het toepassen van een licentie.

```csharp
public class License
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [License](license)() | Initialiseer een exemplaar van de License-klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense)(Stream) | Stelt de GroupDocs.Redaction-licentie in vanuit een stream. |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense_1)(string) | Stelt de GroupDocs.Redaction-licentie in vanuit een bestandspad. |

### Opmerkingen

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Voorbeelden

Het volgende voorbeeld laat zien hoe de licentie voor GroupDocs.Redaction kan worden ingesteld.

```csharp
GroupDocs.Redaction.License license = new GroupDocs.Redaction.License();
// Als alternatief kun je een stream gebruiken:
license.SetLicense(licensePath);
```

### Zie ook

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
