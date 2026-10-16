---
title: "GroupDocs.Redaction.Integration"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Το namespace Integration παρέχει διεπαφές και κλάσεις που χρησιμοποιούνται για την ενσωμάτωση εγγράφων διαφορετικών μορφών με το GroupDocs.Redaction."
type: docs
weight: 40
url: /el/net/groupdocs.redaction.integration/
---
Το namespace Integration παρέχει διεπαφές και κλάσεις, που χρησιμοποιούνται για την ενσωμάτωση εγγράφων διαφορετικών μορφών με το GroupDocs.Redaction.

## Κλάσεις

| Κλάση | Περιγραφή |
| --- | --- |
| [DocumentFormatInstance](./documentformatinstance) | Αντιπροσωπεύει μια συγκεκριμένη μορφή εγγράφου. Υλοποιήστε αυτήν την κλάση για να προσθέσετε τους δικούς σας τύπους εγγράφων. |
| [MetadataCollection](./metadatacollection) | Αντιπροσωπεύει ένα λεξικό του [`MetadataItem`](../groupdocs.redaction.integration/metadataitem) με τον τίτλο του ως κλειδί. |
| [MetadataItem](./metadataitem) | Αντιπροσωπεύει ένα στοιχείο μεταδεδομένων, κοινό για όλες τις υποστηριζόμενες μορφές και χρησιμοποιείται σε διαγραφές μεταδεδομένων. |
## Διεπαφές

| Διεπαφή | Περιγραφή |
| --- | --- |
| [IAnnotatedDocument](./iannotateddocument) | Ορίζει μεθόδους που απαιτούνται για πρόσβαση σε σημειώσεις, όπως σχόλια. Πρέπει να υλοποιηθεί από κλάση που προέρχεται από το [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) για την εκτέλεση διαγραφών σημειώσεων. |
| [ICellularFormatInstance](./icellularformatinstance) | Ορίζει μεθόδους που απαιτούνται για πρόσβαση σε μορφές λογιστικών φύλλων, που έχουν ένα ή πολλά φύλλα εργασίας. |
| [IFixedFormatDocument](./ifixedformatdocument) | Ορίζει μεθόδους που απαιτούνται για μορφές πρόσβασης σταθερής δομής, όπως PDF ή παρουσιάσεις. |
| [IImageFormatInstance](./iimageformatinstance) | Ορίζει μεθόδους που απαιτούνται για διαγραφές μορφής ραστερ εικόνας. |
| [IMetadataAccess](./imetadataaccess) | Ορίζει μεθόδους που απαιτούνται για πρόσβαση στα μεταδεδομένα ενός εγγράφου, εάν η μορφή το υποστηρίζει. |
| [IPaginatedDocument](./ipaginateddocument) | Ορίζει μεθόδους που απαιτούνται για τη διαχείριση των σελίδων ενός εγγράφου. Πρέπει να υλοποιηθεί από κλάση που προέρχεται από το [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) για την εκτέλεση διαγραφών σελίδων. |
| [IPreviewable](./ipreviewable) | Ορίζει μεθόδους για τη δημιουργία προεπισκόπησης του εγγράφου. |
| [IRasterizableDocument](./irasterizabledocument) | Ορίζει μεθόδους που απαιτούνται για την αποθήκευση του εγγράφου σε οποιαδήποτε δυαδική μορφή. Οι ενσωματωμένοι τύποι αποθηκεύουν ένα έγγραφο ως PDF με εικόνες των σελίδων του. |
| [ITextualFormatInstance](./itextualformatinstance) | Ορίζει μεθόδους που απαιτούνται για τη διαγραφή κειμενικών δεδομένων σε οποιοδήποτε έγγραφο που περιέχει κείμενο. |

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
