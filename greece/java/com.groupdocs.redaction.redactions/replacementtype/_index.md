---
title: "ReplacementType"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει έναν τύπο αντικατάστασης για το ταιριασμένο κείμενο."
type: docs
weight: 38
url: /el/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Αντιπροσωπεύει έναν τύπο αντικατάστασης για το ταιριασμένο κείμενο.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Αντικαθιστά το ταιριασμένο κείμενο με άλλη συμβολοσειρά, π.χ. |
|
|  | [DrawBox](#DrawBox) | Σχεδιάζει ένα ορθογώνιο συγκεκριμένου χρώματος (Μαύρο εξ ορισμού) αντί για το κείμενο που έχει αφαιρεθεί. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Αντικαθιστά το ταιριασμένο κείμενο με άλλη συμβολοσειρά, π.χ. κωδικός εξαίρεσης.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Σχεδιάζει ένα ορθογώνιο συγκεκριμένου χρώματος (Μαύρο εξ ορισμού) αντί για το κείμενο που έχει αφαιρεθεί.


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
