---
title: "ページのレダクションを削除"
linkTitle: "Remove page redactions"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "この記事では、PDF、プレゼンテーション、スプレッドシート文書から機密データを含むページを削除する方法を示します。"
type: docs
url: /ja/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction を使用すると、PDF 文書のページ、プレゼンテーションのスライド、スプレッドシートのワークシートを簡単に削除できます。

GroupDocs.Redaction API を使用すると、ページ範囲を相対位置（開始または終了）、ゼロベースインデックス、削除するページ数で指定してページを削除できます。現在サポートされている形式は、PDF、プレゼンテーション（Microsoft PowerPoint、OpenOffice プレゼンテーション）、ワードプロセッシング文書（Microsoft Word、OpenOffice テキスト、リッチテキストファイル）、スプレッドシート（Microsoft Excel、OpenOffice スプレッドシートなど）およびマルチフレーム画像です。

## Remove page range

以下の例では、文書に十分なページがある場合、2 ページ目、3 ページ目、4 ページ目を削除します。

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # レダクト対象のドキュメントをロードします
    with Redactor("./multipage_sample.pdf") as redactor:
        # 文書情報を取得
        doc_info = redactor.get_document_info()

        # 最低 4 ページが必要です
        if doc_info.page_count > 3:
            # 2 ページ目（ゼロベースインデックス 1）から 3 ページを削除
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # 赤字化を適用します
            result = redactor.apply(rem_opt)

            # マスクしたドキュメントを元ファイルの隣に保存する
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` はこの例で使用されるサンプルファイルです。クリック [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) してダウンロードしてください。

## Remove last page

場合によっては、ページ数に関係なく、最後のページや複数のページを削除する必要があることがあります。

次の例は、文書から最後のページを削除する方法を示しています。

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # 文書の末尾から数えて 1 ページを削除します
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # レダクト対象のドキュメントをロードします
    with Redactor("./multipage_sample.pdf") as redactor:
        # 文書情報を取得
        doc_info = redactor.get_document_info()

        # 文書が空にならないように、最低 2 ページが必要です
        if doc_info.page_count > 1:
            # 赤字化を適用します
            result = redactor.apply(rem_opt)

            # マスクしたドキュメントを元ファイルの隣に保存する
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` はこの例で使用されるサンプルファイルです。クリック [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) してダウンロードしてください。

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

マルチフレーム画像の場合、フレーム（「ページ」とみなされます）を複数削除する必要があるかもしれません。

次の例は、アニメーション GIF 画像から 3 フレームを削除する方法を示しています。

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # 3 フレーム目（ゼロベースインデックス 2）からフレームを削除
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # レダクション対象のマルチフレーム画像を読み込む
    with Redactor("./sample.gif") as redactor:
        # 文書情報を取得
        doc_info = redactor.get_document_info()

        # 最低 7 フレームが必要です
        if doc_info.page_count >= 7:
            # 赤字化を適用します
            result = redactor.apply(rem_opt)

            # レダクションされた画像を元ファイルの隣に保存する
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` はこの例で使用されるサンプルファイルです。クリック [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) してダウンロードしてください。

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
