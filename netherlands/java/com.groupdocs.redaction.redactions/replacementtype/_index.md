---
title: "ReplacementType"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Vertegenwoordigt een type vervanging voor de gematchte tekst."
type: docs
weight: 38
url: /nl/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Vertegenwoordigt een type vervanging voor de gematchte tekst.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Vervangt overeenkomende tekst door een andere string, bijv. |
|
|  | [DrawBox](#DrawBox) | Tekent een rechthoek van een specifieke kleur (Zwart standaard) in plaats van geredigeerde tekst. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Vervangt overeenkomende tekst door een andere string, bijv. vrijstellingscode.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Tekent een rechthoek van een specifieke kleur (Zwart standaard) in plaats van geredigeerde tekst.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
