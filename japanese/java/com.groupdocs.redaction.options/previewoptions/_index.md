---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "プレビュー生成のための要件とストリームデリゲートを設定するオプションを提供します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

プレビュー生成のための要件とストリームデリゲートを設定するオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | PreviewOptions クラスの新しいインスタンスを初期化し、出力ストリームを閉じます。 |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | PreviewOptions クラスの新しいインスタンスを初期化し、出力ストリームをクライアントに返してさらに使用できるようにします。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getWidth()](#getWidth--) | ページプレビューの幅を取得または設定します。 |
|
|  | [setWidth(int value)](#setWidth-int-) | ページプレビューの幅を取得または設定します。 |
|
|  | [getHeight()](#getHeight--) | ページプレビューの高さを取得または設定します。 |
|
|  | [setHeight(int value)](#setHeight-int-) | ページプレビューの高さを取得または設定します。 |
|
|  | [getPageNumbers()](#getPageNumbers--) | プレビューを生成するページ番号の配列を取得または設定します。 |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | プレビューを生成するページ番号の配列を取得または設定します。 |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | プレビュー画像の形式を取得または設定します。 |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | プレビュー画像の形式を取得または設定します。 |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | ページストリーム作成デリゲートのインスタンスを取得または設定します。 |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | ページストリーム作成デリゲートのインスタンスを取得または設定します。 |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | ページプレビュー完了デリゲートのインスタンスを取得または設定します。 |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | ページプレビュー完了デリゲートのインスタンスを取得または設定します。 |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


PreviewOptions クラスの新しいインスタンスを初期化し、出力ストリームを閉じます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | 特定のページプレビュー用のストリームを作成します |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


PreviewOptions クラスの新しいインスタンスを初期化し、出力ストリームをクライアントに返してさらに使用できるようにします。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | 特定のページプレビュー用のストリームを作成します |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | ページプレビューの生成が完了したことを通知し、出力ストリームを取得します |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


ページプレビューの幅を取得または設定します。


**Returns:**
int - ページプレビューの幅。

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


ページプレビューの幅を取得または設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | ページプレビューの幅。 |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


ページプレビューの高さを取得または設定します。


**Returns:**
int - ページプレビューの高さ。

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


ページプレビューの高さを取得または設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | ページプレビューの高さ。 |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


プレビューを生成するページ番号の配列を取得または設定します。


**Returns:**
int[] - プレビューを生成するページ番号の配列。

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


プレビューを生成するページ番号の配列を取得または設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int[] | プレビューを生成するページ番号の配列。 |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


プレビュー画像の形式を取得または設定します。


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


プレビュー画像の形式を取得または設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | プレビュー画像の形式。 |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


ページストリーム作成デリゲートのインスタンスを取得または設定します。


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


ページストリーム作成デリゲートのインスタンスを取得または設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | ページストリーム作成デリゲートのインスタンス。 |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


ページプレビュー完了デリゲートのインスタンスを取得または設定します。


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


ページプレビュー完了デリゲートのインスタンスを取得または設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | ページプレビュー完了デリゲートのインスタンス。 |
|

