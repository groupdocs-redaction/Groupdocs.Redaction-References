---
title: Redactor
second_title: GroupDocs.Redaction for .NET API リファレンス
description: の新しいインスタンスを初期化しますRedactorgroupdocs.redaction/redactorファイルパスを使用するクラス.
type: docs
weight: 10
url: /ja/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

の新しいインスタンスを初期化します[`Redactor`](../../redactor)ファイルパスを使用するクラス.

```csharp
public Redactor(string filePath)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルへのパス |

### 例

次の例は、墨消しのためにドキュメントを開く方法を示しています。

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // ここで、ドキュメント インスタンスを使用してリダクションを実行できます
}
```

### 関連項目

* class [Redactor](../../redactor)
* 名前空間 [GroupDocs.Redaction](../../redactor)
* 組み立て [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

の新しいインスタンスを初期化します[`Redactor`](../../redactor) stream. を使用したクラス

```csharp
public Redactor(Stream document)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| document | Stream | ドキュメントのソース ストリーム |

### 例

次の例は、ストリームからドキュメントを開く方法を示しています。

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // ここで、ドキュメント インスタンスを使用してリダクションを実行できます
    }
}
```

### 関連項目

* class [Redactor](../../redactor)
* 名前空間 [GroupDocs.Redaction](../../redactor)
* 組み立て [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

の新しいインスタンスを初期化します[`Redactor`](../../redactor) path. を使用した、パスワードで保護されたドキュメントのクラス

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルへのパス。 |
| loadOptions | LoadOptions | パスワードを含むオプション。 |

### 関連項目

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* 名前空間 [GroupDocs.Redaction](../../redactor)
* 組み立て [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

の新しいインスタンスを初期化します[`Redactor`](../../redactor)パスと設定を使用して、パスワードで保護されたドキュメントのクラス.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| filePath | String | ファイルへのパス。 |
| loadOptions | LoadOptions | パスワードを含むファイル依存のオプション。 |
| settings | RedactorSettings | リダクション プロセスのデフォルト設定。 |

### 関連項目

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* 名前空間 [GroupDocs.Redaction](../../redactor)
* 組み立て [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

の新しいインスタンスを初期化します[`Redactor`](../../redactor) stream. を使用したパスワードで保護されたドキュメントのクラス

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| document | Stream | ソース入力ストリーム。 |
| loadOptions | LoadOptions | パスワードを含むオプション。 |

### 例

次の例は、LoadOptions を使用してパスワードで保護されたドキュメントを開く方法を示しています。

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // ここで、ドキュメント インスタンスを使用してリダクションを実行できます
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* 名前空間 [GroupDocs.Redaction](../../redactor)
* 組み立て [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

の新しいインスタンスを初期化します[`Redactor`](../../redactor)stream と settings. を使用した、パスワードで保護されたドキュメントのクラス

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| document | Stream | ソース入力ストリーム。 |
| loadOptions | LoadOptions | パスワードを含むオプション。 |
| settings | RedactorSettings | リダクション プロセスのデフォルト設定。 |

### 例

次の例は、LoadOptions を使用してパスワードで保護されたドキュメントを開く方法を示しています。

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // ここで、ドキュメント インスタンスを使用してリダクションを実行できます
}
```

### 関連項目

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* 名前空間 [GroupDocs.Redaction](../../redactor)
* 組み立て [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
