---
title: "ReplacementType"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет тип замены для найденного текста."
type: docs
weight: 38
url: /ru/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Представляет тип замены для найденного текста.

## Поля

| Поле | Описание |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Заменяет найденный текст другой строкой, например. |
|
|  | [DrawBox](#DrawBox) | Рисует прямоугольник определённого цвета (по умолчанию чёрный) вместо редактируемого текста. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Заменяет найденный текст другой строкой, например код освобождения.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Рисует прямоугольник определённого цвета (по умолчанию чёрный) вместо редактируемого текста.


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
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
