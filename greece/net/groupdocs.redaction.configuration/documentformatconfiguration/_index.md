---
title: DocumentFormatConfiguration
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Αντιπροσωπεύει μια αναφορά τύπου γιαDocumentFormatInstance../groupdocs.redaction.integration/documentformatinstance προερχόμενη κλάση και λίστα υποστηριζόμενων επεκτάσεων αρχείων για ταχύτερο εντοπισμό μορφής.
type: docs
weight: 10
url: /el/net/groupdocs.redaction.configuration/documentformatconfiguration/
---
## DocumentFormatConfiguration class

Αντιπροσωπεύει μια αναφορά τύπου για[`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) -προερχόμενη κλάση και λίστα υποστηριζόμενων επεκτάσεων αρχείων για ταχύτερο εντοπισμό μορφής.

```csharp
public class DocumentFormatConfiguration
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [DocumentFormatConfiguration](documentformatconfiguration)() | Αρχικοποιεί μια νέα παρουσία της κλάσης DocumentFormatConfiguration. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [DocumentType](../../groupdocs.redaction.configuration/documentformatconfiguration/documenttype) { get; set; } | Λαμβάνει ή ορίζει τον τύπο μιας κλάσης, από την οποία κληρονομείται[`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) . |
| [ExtensionFilter](../../groupdocs.redaction.configuration/documentformatconfiguration/extensionfilter) { get; set; } | Λαμβάνει ή ορίζει μια λίστα οριοθετημένη με κόμμα (",") επεκτάσεων αρχείων (για παράδειγμα ".pdf"), χωρίς διάκριση πεζών-κεφαλαίων. |
| [InitializationData](../../groupdocs.redaction.configuration/documentformatconfiguration/initializationdata) { get; set; } | Λαμβάνει ή ορίζει δεδομένα που απαιτούνται για[`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) αρχικοποίηση. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [SupportsExtension](../../groupdocs.redaction.configuration/documentformatconfiguration/supportsextension)(string) | Ελέγχει εάν μια δεδομένη επέκταση αρχείου μπορεί να χειριστεί ως DocumentType. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* Περισσότερες λεπτομέρειες για**GroupDocs.Διαμόρφωση** διαμόρφωση: [Επέκταση της λίστας υποστηριζόμενων επεκτάσεων](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* Περισσότερες λεπτομέρειες σχετικά με την εφαρμογή προσαρμοσμένων μορφών: [Δημιουργία προσαρμοσμένου χειριστή μορφών](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να ορίσετε ιδιότητες για μια προσαρμοσμένη διαμόρφωση μορφής.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
```

### Δείτε επίσης

* χώρος ονομάτων [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
