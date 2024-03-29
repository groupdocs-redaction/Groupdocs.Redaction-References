---
title: GroupDocs.Redaction.Redactions
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: ΤοRedactions Ο χώρος ονομάτων παρέχει κλάσεις για διαφορετικούς τύπους διορθώσεων.
type: docs
weight: 70
url: /el/net/groupdocs.redaction.redactions/
---
ΤοRedactions Ο χώρος ονομάτων παρέχει κλάσεις για διαφορετικούς τύπους διορθώσεων.

## Τάξεις

| Τάξη | Περιγραφή |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | Αντιπροσωπεύει μια επεξεργασία που αντικαθιστά το κείμενο σχολιασμού (σχόλια, κ.λπ.) που ταιριάζει με μια δεδομένη κανονική έκφραση. |
| [CellColumnRedaction](./cellcolumnredaction) | Αντιπροσωπεύει μια επεξεργασία κειμένου που αντικαθιστά κείμενο σε έγγραφα υπολογιστικού φύλλου (CSV, Excel, κ.λπ.). |
| [CellFilter](./cellfilter) | Παρέχει μια επιλογή για τον περιορισμό του εύρους του a[`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) σε ένα φύλλο εργασίας και μια στήλη. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | Αντιπροσωπεύει μια επεξεργασία κειμένου που διαγράφει σχολιασμούς εάν το κείμενο ταιριάζει με δεδομένη κανονική έκφραση (προαιρετικά διαγράφει όλους τους σχολιασμούς). |
| [EraseMetadataRedaction](./erasemetadataredaction) | Αντιπροσωπεύει μια επεξεργασία μεταδεδομένων που διαγράφει όλα τα μεταδεδομένα ή τα μεταδεδομένα που αντιστοιχούν σε συγκεκριμένα φίλτρα μεταδεδομένων από το έγγραφο. |
| [ExactPhraseRedaction](./exactphraseredaction) | Αντιπροσωπεύει μια επεξεργασία κειμένου που αντικαθιστά την ακριβή φράση στο κείμενο του εγγράφου, χωρίς διάκριση πεζών-κεφαλαίων από προεπιλογή. |
| [ImageAreaRedaction](./imagearearedaction) | Αντιπροσωπεύει μια διόρθωση που τοποθετεί έγχρωμο ορθογώνιο σε δεδομένη περιοχή ενός εγγράφου εικόνας. |
| [MetadataRedaction](./metadataredaction) | Αντιπροσωπεύει μια βασική αφηρημένη κλάση για διορθώσεις μεταδεδομένων εγγράφων. |
| [MetadataSearchRedaction](./metadatasearchredaction) | Αντιπροσωπεύει μια επεξεργασία μεταδεδομένων που πραγματοποιεί αναζήτηση και διόρθωση μεταδεδομένων χρησιμοποιώντας κανονικές εκφράσεις, αντιστοιχισμένα κλειδιά και/ή τιμές. |
| [RedactionDescription](./redactiondescription) | Αντιπροσωπεύει μια ενιαία πληροφορία ενέργειας αλλαγής που εκτελέστηκε κατά τη διαδικασία σύνταξης. |
| [RegexRedaction](./regexredaction) | Αντιπροσωπεύει μια επεξεργασία κειμένου που αναζητά και αντικαθιστά κείμενο στο έγγραφο αντιστοιχίζοντας την παρεχόμενη κανονική έκφραση. |
| [RegionReplacementOptions](./regionreplacementoptions) | Αντιπροσωπεύει τις παραμέτρους χρώματος και περιοχής για αντικατάσταση περιοχής εικόνας. Βλέπω[`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction) . |
| [RemovePageRedaction](./removepageredaction) | Αντιπροσωπεύει μια διόρθωση που αφαιρεί μια σελίδα (διαφάνεια, φύλλο εργασίας, κ.λπ.) από ένα έγγραφο. |
| [ReplacementOptions](./replacementoptions) | Αντιπροσωπεύει επιλογές για αντικατάσταση αντιστοιχισμένου κειμένου. |
| [TextRedaction](./textredaction) | Αντιπροσωπεύει μια βασική αφηρημένη κλάση για διορθώσεις κειμένου εγγράφου. |
| [TextReplacement](./textreplacement) | Αντιπροσωπεύει μια πληροφορία αντικατάστασης κειμένου. |
## Διεπαφές

| Διεπαφή | Περιγραφή |
| --- | --- |
| [IRedactionCallback](./iredactioncallback) | Καθορίζει μεθόδους που απαιτούνται για τη λήψη πληροφοριών για κάθε αλλαγή έκδοσης και προαιρετικά την αποτρέπει. |
## Απαρίθμηση

| Απαρίθμηση | Περιγραφή |
| --- | --- |
| [MetadataFilters](./metadatafilters) | Αντιπροσωπεύει μια λίστα με τους πιο συνηθισμένους τύπους μεταδεδομένων εγγράφων. |
| [PageSeekOrigin](./pageseekorigin) | Παρέχει τα πεδία που αντιπροσωπεύουν σημεία αναφοράς σε ένα έγγραφο για αναζήτηση. |
| [RedactionActionType](./redactionactiontype) | Αντιπροσωπεύει ενέργειες που μπορούν να γίνουν για την εκτέλεση της επεξεργασίας. |
| [RedactionType](./redactiontype) | Αντιπροσωπεύει έναν τύπο δεδομένων ενός εγγράφου, που επηρεάζεται από τη διόρθωση. |
| [ReplacementType](./replacementtype) | Αντιπροσωπεύει έναν τύπο αντικατάστασης για το αντιστοιχισμένο κείμενο. |

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
