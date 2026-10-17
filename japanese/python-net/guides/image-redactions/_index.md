---
title: "画像の編集"
linkTitle: "Image redactions"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "この記事では、JPG、PNG、TIFF などのさまざまな形式の画像から機密データを編集する方法を示します。"
type: docs
url: /ja/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions は、JPG、PNG、TIFF などのさまざまな形式の画像から機密データを編集する機能を提供します。完全な一覧は [サポートされているドキュメント形式]() 記事をご覧ください。

GroupDocs.Redaction は、画像を別々の画像ファイルとして、または埋め込み画像として編集する 2 つの方法をサポートしています:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction for Python via .NET は、画像メタデータの変更も可能です（例: 画像の EXIF データを編集したり、\"EXIF イレイサー\" として機能させたり）。

## Redact image area

画像領域を編集するには、[ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) クラスを使用する必要があります:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # 編集する領域の左上位置を定義します
    sample_point = Point(385, 485)
    # 編集が必要な領域のサイズを定義します
    sample_size = Size(1793, 2069)
    # 赤字化ボックスの色を定義する
    color = Color.from_argb(255, 220, 20, 60)

    # レダクションオプションを指定する
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.jpg") as redactor:
        # 赤字化を適用します
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # デフォルトでは、レダクションされたドキュメントは PDF 形式で保存されます
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` はこの例で使用されるサンプルファイルです。[ここ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) をクリックしてダウンロードしてください。

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

この種のファイル（例: 埋め込み画像のない MS Word ドキュメント）に編集を適用できない場合、[RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) は [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) になります。

## Clean image metadata

次の例は、写真やその他の画像から EXIF データを編集（消去）する方法を示しています:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # すべての画像メタデータ（例: EXIF）を削除する編集オプションを指定します
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # 編集対象の画像をロードします
    with Redactor("./sample.jpg") as redactor:
        # 赤字化を適用します
        result = redactor.apply(er_opt)

        # レダクションされた画像を元ファイルの隣に保存する
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` はこの例で使用されるサンプルファイルです。[ここ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) をクリックしてダウンロードしてください。

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

この種のファイル（例: BMP 画像）に編集を適用できない場合、[RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) は [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) になります。

## Redact embedded images

ドキュメント内のすべての埋め込み画像に対して画像領域を編集できます。

次の例は、Microsoft Word ドキュメント内のすべての埋め込み画像を編集する方法を示しています:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # 編集する領域の左上位置を定義します
    sample_point = Point(516, 311)
    # 編集が必要な領域のサイズを定義します
    sample_size = Size(170, 35)
    # 赤字化ボックスの色を定義する
    color = Color.from_argb(255, 220, 20, 60)

    # レダクションオプションを指定する
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # レダクト対象のドキュメントをロードします
    with Redactor("./sample.docx") as redactor:
        # すべての埋め込み画像に編集を適用する
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # デフォルトでは、レダクションされたドキュメントは PDF 形式で保存されます
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` はこの例で使用されるサンプルファイルです。[ここ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) をクリックしてダウンロードしてください。

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

この種のファイル（例: スプレッドシートドキュメント）に編集を適用できない場合、[RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) は [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) になります。

## Multi-frame images

指定された原点とフレーム数でマルチフレーム画像からフレームを削除できます。詳細については [ページ削除の編集]() 記事をご覧ください。

DjVu ドキュメントなどの一部の画像形式は、[事前ラスタライズ]() が必要で、さらに PDF 形式で保存する必要があります。
