---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PreviewOptions προκαλώντας το κλείσιμο της ροής εξόδου."
type: docs
weight: 10
url: /el/net/groupdocs.redaction.options/previewoptions/previewoptions/
---
## PreviewOptions(CreatePageStream) {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PreviewOptions, προκαλώντας το κλείσιμο της ροής εξόδου.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| createPageStream | CreatePageStream | Δημιουργεί μια ροή για μια συγκεκριμένη προεπισκόπηση σελίδας |

### Δείτε επίσης

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης PreviewOptions, προκαλώντας την επιστροφή της ροής εξόδου στον πελάτη για περαιτέρω χρήση.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| createPageStream | CreatePageStream | Δημιουργεί μια ροή για μια συγκεκριμένη προεπισκόπηση σελίδας |
| releasePageStream | ReleasePageStream | Ειδοποιεί ότι η δημιουργία της προεπισκόπησης σελίδας ολοκληρώθηκε και λαμβάνει τη ροή εξόδου |

### Δείτε επίσης

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
