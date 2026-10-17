---
title: "License"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tillhandahåller metoder för att tillämpa licens."
type: docs
weight: 270
url: /sv/net/groupdocs.redaction/license/
---
## License class

Tillhandahåller metoder för att tillämpa licens.

```csharp
public class License
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [License](license)() | Initierar en instans av License-klassen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense)(Stream) | Ställer in GroupDocs.Redaction-licensen från en ström. |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense_1)(string) | Ställer in GroupDocs.Redaction-licensen från en filsökväg. |

### Anmärkningar

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Exempel

Följande exempel visar hur man ställer in licensen för GroupDocs.Redaction.

```csharp
GroupDocs.Redaction.License license = new GroupDocs.Redaction.License();
// som ett alternativ kan du använda en ström:
license.SetLicense(licensePath);
```

### Se även

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
