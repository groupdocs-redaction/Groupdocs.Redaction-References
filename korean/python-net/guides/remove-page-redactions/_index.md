---
title: "페이지 레드액션 제거"
linkTitle: "Remove page redactions"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이 문서는 PDF, 프레젠테이션 및 스프레드시트 문서에서 민감한 데이터가 포함된 페이지를 제거하는 방법을 보여줍니다."
type: docs
url: /ko/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction을 사용하면 PDF 문서의 페이지, 프레젠테이션 슬라이드 및 스프레드시트 워크시트를 쉽게 제거할 수 있습니다.

GroupDocs.Redaction API를 사용하면 페이지 범위를 상대 위치(시작 또는 끝), 0부터 시작하는 인덱스 및 제거할 페이지 수로 지정하여 페이지를 제거할 수 있습니다. 현재 지원되는 형식은 PDF, 프레젠테이션(Microsoft PowerPoint, OpenOffice Presentations), 워드 프로세싱 문서(Microsoft Word, OpenOffice Texts, Rich Text Files), 스프레드시트(Microsoft Excel, OpenOffice Spreadsheets 등) 및 다중 프레임 이미지입니다.

## Remove page range

아래 예제에서는 문서에 충분한 페이지가 있는 경우 두 번째, 세 번째 및 네 번째 페이지를 제거합니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # 레드랙션할 문서를 로드합니다
    with Redactor("./multipage_sample.pdf") as redactor:
        # 문서 정보 가져오기
        doc_info = redactor.get_document_info()

        # 최소 4페이지가 필요합니다
        if doc_info.page_count > 3:
            # 두 번째 페이지(0부터 시작하는 인덱스 1)부터 시작하여 3페이지를 제거합니다
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # 가리기를 적용합니다
            result = redactor.apply(rem_opt)

            # 편집된 문서를 원본 파일 옆에 저장합니다
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf)를 클릭하십시오.

## Remove last page

일부 경우에는 페이지 수에 관계없이 마지막 페이지나 여러 페이지를 삭제해야 할 수 있습니다.

다음 예제는 문서에서 마지막 페이지를 제거하는 방법을 보여줍니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # 문서 끝에서부터 1페이지를 제거합니다
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./multipage_sample.pdf") as redactor:
        # 문서 정보 가져오기
        doc_info = redactor.get_document_info()

        # 문서가 비어 있지 않도록 최소 2페이지가 필요합니다
        if doc_info.page_count > 1:
            # 가리기를 적용합니다
            result = redactor.apply(rem_opt)

            # 편집된 문서를 원본 파일 옆에 저장합니다
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf)를 클릭하십시오.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

다중 프레임 이미지의 경우 여러 프레임(“페이지”로 간주)을 삭제해야 할 수 있습니다.

다음 예제는 애니메이션 GIF 이미지에서 3개의 프레임을 제거하는 방법을 보여줍니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # 세 번째 프레임(0부터 시작하는 인덱스 2)부터 시작하여 프레임을 제거합니다
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # 레드액션할 다중 프레임 이미지를 로드합니다
    with Redactor("./sample.gif") as redactor:
        # 문서 정보 가져오기
        doc_info = redactor.get_document_info()

        # 최소 7개의 프레임이 필요합니다
        if doc_info.page_count >= 7:
            # 가리기를 적용합니다
            result = redactor.apply(rem_opt)

            # 레드액션된 이미지를 원본 파일 옆에 저장합니다
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif)를 클릭하십시오.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
