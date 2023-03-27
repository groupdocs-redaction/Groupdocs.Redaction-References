---
title: FileType
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Αντιπροσωπεύει έναν τύπο αρχείου. Παρέχει μεθόδους για τη λήψη μιας λίστας όλων των τύπων αρχείων που υποστηρίζονται από το GroupDocs.Redaction εντοπισμός τύπου αρχείου κατά επέκταση κ.λπ.
type: docs
weight: 90
url: /el/net/groupdocs.redaction/filetype/
---
## FileType class

Αντιπροσωπεύει έναν τύπο αρχείου. Παρέχει μεθόδους για τη λήψη μιας λίστας όλων των τύπων αρχείων που υποστηρίζονται από το GroupDocs.Redaction, εντοπισμός τύπου αρχείου κατά επέκταση κ.λπ.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Αρχείο εικόνας Bitmap (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Αρχείο τιμών διαχωρισμένων με κόμματα (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Έγγραφο Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Έγγραφο με δυνατότητα μακροεντολής XML Open Word (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML Document (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Πρότυπο εγγράφου Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Πρότυπο εγγράφου ανοιχτού τύπου XML με μακροεντολή (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Πρότυπο εγγράφου Word Open XML (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Αρχείο μορφής γραφικής ανταλλαγής (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Αρχείο γλώσσας σήμανσης υπερκειμένου (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Αρχείο γλώσσας σήμανσης υπερκειμένου (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | Αρχείο εικόνας πυρήνα JPEG 2000 (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Εικόνα JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Εικόνα JPEG (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Αρχείο τεκμηρίωσης Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Υπολογιστικό φύλλο Apple Numbers (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Παρουσίαση OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | Υπολογιστικό φύλλο OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | Έγγραφο κειμένου OpenDocument (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Πρότυπο υπολογιστικού φύλλου OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Πρότυπο εγγράφου OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Φορητό αρχείο μορφής εγγράφου (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Φορητό γραφικό δικτύου (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Παρουσίαση PowerPoint (.ppt) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Άνοιγμα παρουσίασης XML (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Αρχείο μορφής εμπλουτισμένου κειμένου (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Αρχείο εικόνας με ετικέτα (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Μορφή αρχείου εικόνας με ετικέτα (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Αρχείο τιμών διαχωρισμένων με καρτέλες (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Αρχείο απλού κειμένου (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Αντιπροσωπεύει άγνωστο τύπο αρχείου. |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Υπολογιστικό φύλλο Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Δυαδικό υπολογιστικό φύλλο Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML Macro-Enabled Spreadsheet (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Άνοιγμα υπολογιστικού φύλλου XML (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Λαμβάνει επίθημα ονόματος αρχείου (συμπεριλαμβανομένης της περιόδου "."), για παράδειγμα ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Λαμβάνει όνομα τύπου αρχείου, για παράδειγμα "Microsoft Word Document". |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Επέκταση αρχείου Χαρτών στον τύπο αρχείου. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Καθορίζει εάν το ρεύμα[`FileType`](../filetype) είναι το ίδιο με αυτό που ορίζεται[`FileType`](../filetype) αντικείμενο. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Καθορίζει εάν το ρεύμα[`FileType`](../filetype) είναι το ίδιο με το καθορισμένο αντικείμενο. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Επιστρέφει τον κωδικό κατακερματισμού για το τρέχον[`FileType`](../filetype) αντικείμενο. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Ανακτά τους υποστηριζόμενους τύπους αρχείων |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Καθορίζει αν δύο[`FileType`](../filetype) τα αντικείμενα είναι ίδια. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Καθορίζει αν δύο[`FileType`](../filetype) τα αντικείμενα δεν είναι ίδια. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* [Υποστηριζόμενες μορφές εγγράφων](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Λάβετε υποστηριζόμενες μορφές αρχείων](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Λάβετε πληροφορίες αρχείου](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Δείτε επίσης

* χώρος ονομάτων [GroupDocs.Redaction](../../groupdocs.redaction)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
