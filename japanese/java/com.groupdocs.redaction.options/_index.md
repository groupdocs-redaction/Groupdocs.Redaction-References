---
title: "com.groupdocs.redaction.options"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "このパッケージは、ロードおよび保存オプションのクラスを提供します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.redaction.options/
---

このパッケージは、ロードおよび保存オプションのクラスを提供します。



## クラス

| クラス | 説明 |
| --- | --- |
| [LoadOptions](../com.groupdocs.redaction.options/loadoptions) | ファイルを開く際に使用されるオプションを提供します。 |
| [PreviewOptions](../com.groupdocs.redaction.options/previewoptions) | プレビュー生成のための要件とストリームデリゲートを設定するオプションを提供します。 |
| [RasterizationOptions](../com.groupdocs.redaction.options/rasterizationoptions) | ファイルを PDF に変換するためのオプションを提供します。 |
| [RedactorSettings](../com.groupdocs.redaction.options/redactorsettings) | 赤字設定を表し、赤字プロセスをカスタマイズできるようにします。 |
| [SaveOptions](../com.groupdocs.redaction.options/saveoptions) | 出力ファイル名の変更や、ドキュメントを画像ベースの PDF（ラスタライズ）に変換するオプションを提供します。 |
| [WordprocessingSaveOptions](../com.groupdocs.redaction.options/wordprocessingsaveoptions) | ワードプロセッシングの保存オプション。 |

## インターフェイス

| インターフェイス | 説明 |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.redaction.options/icreatepagestream) | ページプレビュー データを書き込むためのストリームを返すメソッドを提供します。 |
| [ILogger](../com.groupdocs.redaction.options/ilogger) | 赤字プロセスでイベントやエラーを記録するために使用できるロガーのインターフェイスを定義します。 |
| [IReleasePageStream](../com.groupdocs.redaction.options/ireleasepagestream) | CreatePageStream デリゲートによって作成されたストリームを解放するメソッドを表します。 |

## 列挙型

| 列挙型 | 説明 |
| --- | --- |
| [AdvancedRasterizationOptions](../com.groupdocs.redaction.options/advancedrasterizationoptions) | 適用される高度なラスタライズオプションを管理する列挙型です。 |
| [PdfComplianceLevel](../com.groupdocs.redaction.options/pdfcompliancelevel) | サポートされている PDF 準拠レベルの一覧を表します。 |
| [PreviewFormats](../com.groupdocs.redaction.options/previewformats) | サポートされているプレビュー形式を表します。 |
| [WordProcessingComplianceLevel](../com.groupdocs.redaction.options/wordprocessingcompliancelevel) | ワードプロセッシング ドキュメントの OOXML 準拠レベル。 |
