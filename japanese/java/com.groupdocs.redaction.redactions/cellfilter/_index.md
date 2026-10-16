---
title: "CellFilter"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "CellColumnRedaction の対象範囲をワークシートと列に限定するオプションを提供します。"
type: docs
weight: 12
url: /ja/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

範囲を制限するオプションを提供します
CellColumnRedaction
ワークシートと列に対して。

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | 新しいインスタンスを初期化します。 |
|
## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [NoIndex](#NoIndex) | フィルターのデフォルト値（-1）を表します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | ワークシート名を取得します（該当する場合）。 |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | ワークシート名を設定します（該当する場合）。 |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | ワークシートインデックスを取得します（ゼロベース）。 |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | ワークシートインデックスを設定します（ゼロベース）。 |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | 設定されているかどうかを示す値を取得します |
WorkSheetIndex
設定されているかどうか。
|
|  | [getColumnIndex()](#getColumnIndex--) | 列インデックスを取得します（ゼロベース）。 |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | 列インデックスを設定します（ゼロベース）。 |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


新しいインスタンスを初期化します。


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


フィルターのデフォルト値（-1）を表します。


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


ワークシート名を取得します（該当する場合）。


**Returns:**
java.lang.String - ワークシート名（該当する場合）。

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


ワークシート名を設定します（該当する場合）。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | ワークシート名（該当する場合）。 |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


ワークシートインデックスを取得します（ゼロベース）。


**Returns:**
int - ワークシートインデックス（ゼロベース）。

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


ワークシートインデックスを設定します（ゼロベース）。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | ワークシートインデックス（ゼロベース）。 |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


設定されているかどうかを示す値を取得します
WorkSheetIndex
設定されているかどうか。


**Returns:**
boolean - WorkSheetIndex が設定されているかどうかを示す値です。

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


列インデックスを取得します（ゼロベース）。


**Returns:**
int - 列インデックス（ゼロベース）。

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


列インデックスを設定します（ゼロベース）。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | 列インデックス（ゼロベース）。 |
|

