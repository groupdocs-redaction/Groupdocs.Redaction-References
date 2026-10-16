---
title: "MetadataItem"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "すべてのサポートされている形式で共通のメタデータ項目を表し、メタデータの編集に使用されます。"
type: docs
weight: 12
url: /ja/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

すべてのサポート対象フォーマットで共通のメタデータ項目を表し、メタデータの編集に使用されます。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | 新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | ドキュメントに表示されるメタデータ項目の元の名前を取得します。 |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | ドキュメントに表示されるメタデータ項目の元の名前を設定します。 |
|
|  | [getCategory()](#getCategory--) | 埋め込みリソースのメタデータ項目のリソースIDなど、メタデータ項目のカテゴリを取得します。 |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | 埋め込みリソースのメタデータ項目のリソースIDなど、メタデータ項目のカテゴリを設定します。 |
|
|  | [getFilter()](#getFilter--) | 値を取得します |
MetadataFilters
、このメタデータ項目に割り当てられ、項目のフィルタリングに使用されます。
|
|  | [setFilter(int value)](#setFilter-int-) | 値を設定します |
MetadataFilters
、このメタデータ項目に割り当てられ、項目のフィルタリングに使用されます。
|
|  | [getValues()](#getValues--) | メタデータ項目の値を取得します。 |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | メタデータ項目の値を設定します。 |
|
|  | [isCustom()](#isCustom--) | この項目がカスタムかどうか（ドキュメントの作成者によって追加されたか）を示す値を取得します。 |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | この項目がカスタムかどうか（ドキュメントの作成者によって追加されたか）を示す値を設定します。 |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | OriginalNameやその他のデータを使用して、 の辞書キーを取得します。 |
|
|  | [createClone()](#createClone--) | 現在のインスタンスのディープクローンを作成します。 |
|
|  | [getActualValue()](#getActualValue--) | メタデータ項目の値の文字列表現を取得します。 |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


新しいインスタンスを初期化します。


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


ドキュメントに表示されるメタデータ項目の元の名前を取得します。


**Returns:**
java.lang.String - ドキュメントに表示されるメタデータ項目の元の名前。

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


ドキュメントに表示されるメタデータ項目の元の名前を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | ドキュメントに表示されるメタデータ項目の元の名前。 |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


埋め込みリソースのメタデータ項目のリソースIDなど、メタデータ項目のカテゴリを取得します。


**Returns:**
java.lang.String - 埋め込みリソースのメタデータ項目のリソースIDなど、メタデータ項目のカテゴリ。

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


埋め込みリソースのメタデータ項目のリソースIDなど、メタデータ項目のカテゴリを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | 埋め込みリソースのメタデータ項目のリソースIDなど、メタデータ項目のカテゴリ。 |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


値を取得します
MetadataFilters
、このメタデータ項目に割り当てられ、項目のフィルタリングに使用されます。


**Returns:**
int - MetadataFilters の値で、このメタデータ項目に割り当てられ、項目のフィルタリングに使用されます。

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


値を設定します
MetadataFilters
、このメタデータ項目に割り当てられ、項目のフィルタリングに使用されます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | MetadataFilters の値で、このメタデータ項目に割り当てられ、項目のフィルタリングに使用されます。 |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


メタデータ項目の値を取得します。


**Returns:**
java.util.List<java.lang.String> - メタデータ項目の値。

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


メタデータ項目の値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.util.List<java.lang.String> | メタデータ項目の値。 |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


この項目がカスタムかどうか（ドキュメントの作成者によって追加されたか）を示す値を取得します。


**Returns:**
boolean - この項目がカスタムかどうかを示す値（ドキュメントの作成者によって追加されたもの）。

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


この項目がカスタムかどうか（ドキュメントの作成者によって追加されたか）を示す値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | boolean | この項目がカスタムかどうかを示す値（ドキュメントの作成者によって追加されたもの）。 |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


OriginalNameやその他のデータを使用して、 の辞書キーを取得します。


**Returns:**
java.lang.String - OriginalName などのデータを使用して、 の辞書キー。

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


現在のインスタンスのディープクローンを作成します。


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


メタデータ項目の値の文字列表現を取得します。


**Returns:**
java.lang.String - メタデータ項目値の文字列表現。

