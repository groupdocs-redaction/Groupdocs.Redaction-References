---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει πληροφορίες μιας μοναδικής ενέργειας αλλαγής που εκτελέστηκε κατά τη διαδικασία διαγραφής."
type: docs
weight: 25
url: /el/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Αντιπροσωπεύει πληροφορίες μιας μοναδικής ενέργειας αλλαγής που εκτελέστηκε κατά τη διαδικασία διαγραφής.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionDescription χωρίς πληροφορίες αντικατάστασης. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionDescription με πληροφορίες αντικατάστασης. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionDescription με πληροφορίες αντικατάστασης περιοχής εικόνας. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Ανακτά τον τύπο των δεδομένων του εγγράφου - κείμενο, μεταδεδομένα ή σημειώσεις. |
|
|  | [getActionType()](#getActionType--) | Λαμβάνει τη λειτουργία διαγραφής: αντικατάσταση, καθαρισμός ή διαγραφή. |
|
|  | [getOriginalText()](#getOriginalText--) | Λαμβάνει το αντιστοιχισμένο κείμενο, εάν έχει δοθεί κάποια έκφραση. |
|
|  | [getReplacement()](#getReplacement--) | Λαμβάνει τις πληροφορίες αντικατάστασης, μπορεί να είναι null. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Λαμβάνει τις πληροφορίες αντικατάστασης για περιοχές εικόνας, επιστρέφει null για κειμενικές διαγραφές. |
|
|  | [getDetails()](#getDetails--) | Λαμβάνει προαιρετικές λεπτομερείς πληροφορίες για το αντικείμενο που διαγράφεται. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Ορίζει προαιρετικές λεπτομερείς πληροφορίες για το αντικείμενο που διαγράφεται. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionDescription χωρίς πληροφορίες αντικατάστασης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | redactionType | int | Τύπος των δεδομένων που διαγράφονται |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Δράση που θα εκτελεστεί σε αυτά τα δεδομένα |
|
|  | originalText | java.lang.String | Αντιστοιχισμένο κείμενο, σχόλιο ή σώμα σημείωσης |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionDescription με πληροφορίες αντικατάστασης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | redactionType | int | Τύπος των δεδομένων που διαγράφονται |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Δράση που θα εκτελεστεί σε αυτά τα δεδομένα |
|
|  | originalText | java.lang.String | Αντιστοιχισμένο κείμενο, σχόλιο ή σώμα σημείωσης |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Κείμενο αντικατάστασης, αντιστοιχισμένο κείμενο και η θέση του στο αρχικό κείμενο |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionDescription με πληροφορίες αντικατάστασης περιοχής εικόνας.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | redactionType | int | Τύπος των δεδομένων που διαγράφονται |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Δράση που θα εκτελεστεί σε αυτά τα δεδομένα |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Πληροφορίες αντικατάστασης περιοχής εικόνας |
|
|  | imageDetails | java.lang.String | Περιγραφή κειμένου εικόνας, εξ ορισμού είναι String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Ανακτά τον τύπο των δεδομένων του εγγράφου - κείμενο, μεταδεδομένα ή σημειώσεις.


**Returns:**
int - Ο τύπος των δεδομένων του εγγράφου - κείμενο, μεταδεδομένα ή σημειώσεις.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Λαμβάνει τη λειτουργία διαγραφής: αντικατάσταση, καθαρισμός ή διαγραφή.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Λαμβάνει το αντιστοιχισμένο κείμενο, εάν έχει δοθεί κάποια έκφραση.


**Returns:**
java.lang.String - Το αντιστοιχισμένο κείμενο, εάν έχει δοθεί κάποια έκφραση.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Λαμβάνει τις πληροφορίες αντικατάστασης, μπορεί να είναι null.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Λαμβάνει τις πληροφορίες αντικατάστασης για περιοχές εικόνας, επιστρέφει null για κειμενικές διαγραφές.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Λαμβάνει προαιρετικές λεπτομερείς πληροφορίες για το αντικείμενο που διαγράφεται.


**Returns:**
java.lang.String - Προαιρετικές λεπτομερείς πληροφορίες για το αντικείμενο που διαγράφεται.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Ορίζει προαιρετικές λεπτομερείς πληροφορίες για το αντικείμενο που διαγράφεται.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Προαιρετικές λεπτομερείς πληροφορίες για το αντικείμενο που διαγράφεται. |
|

