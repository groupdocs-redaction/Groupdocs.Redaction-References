---
title: "AnnotationRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en redigering som ersätter annoteringstext, kommentarer etc. som matchar ett givet reguljärt uttryck."
type: docs
weight: 530
url: /sv/net/groupdocs.redaction.redactions/annotationredaction/
---
## AnnotationRedaction class

Representerar en radering som ersätter annoteringstext (kommentarer osv.) som matchar ett givet reguljärt uttryck.

```csharp
public class AnnotationRedaction : Redaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [AnnotationRedaction](annotationredaction#constructor_1)(Regex, string) | Initierar en ny instans av klassen AnnotationRedaction. |
| [AnnotationRedaction](annotationredaction#constructor)(string, string) | Initierar en ny instans av klassen AnnotationRedaction. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/annotationredaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [Expression](../../groupdocs.redaction.redactions/annotationredaction/expression) { get; } | Hämtar det reguljära uttrycket att matcha. |
| [Replacement](../../groupdocs.redaction.redactions/annotationredaction/replacement) { get; } | Hämtar en textuell ersättning för matchad text. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/annotationredaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Exempel

Följande exempel visar hur man ersätter namnet "John" med "[redacted]" i alla annoteringar.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
   redactor.Save()
}
```

### Se även

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
