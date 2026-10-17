---
title: "이미지 가리기"
linkTitle: "Image redactions"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이 문서는 JPG, PNG, TIFF 등 다양한 형식의 이미지에서 민감한 데이터를 가리는 방법을 보여줍니다."
type: docs
url: /ko/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions는 JPG, PNG, TIFF 등 다양한 형식의 이미지에서 민감한 데이터를 가리기 위한 다양한 기능을 제공합니다. 전체 목록은 [supported document formats]() 기사에서 확인하세요.

GroupDocs.Redaction은 이미지 파일 자체와 삽입된 이미지, 두 가지 방식으로 이미지를 가리는 것을 지원합니다:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction for Python via .NET은 이미지 메타데이터를 변경할 수도 있습니다(예: 이미지의 EXIF 데이터를 편집하거나 "EXIF 지우기" 역할 수행).

## Redact image area

이미지 영역을 가리려면 [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) 클래스를 사용해야 합니다:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # 가릴 영역의 좌상단 위치를 정의합니다
    sample_point = Point(385, 485)
    # 가릴 영역의 크기를 정의합니다
    sample_size = Size(1793, 2069)
    # 레드액션 상자의 색상 정의
    color = Color.from_argb(255, 220, 20, 60)

    # 편집 옵션을 지정합니다
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.jpg") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # 기본적으로 레드랙션된 문서는 PDF 형식으로 저장됩니다.
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg)를 클릭하세요.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

이 유형의 파일에 가리기를 적용할 수 없는 경우(예: 삽입된 이미지가 없는 MS Word 문서), [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/)는 [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/)가 됩니다.

## Clean image metadata

다음 예제는 사진이나 기타 이미지에서 EXIF 데이터를 편집(삭제)하는 방법을 보여줍니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # 모든 이미지 메타데이터(EXIF 등)를 제거하기 위한 가리기 옵션을 지정합니다
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # 가릴 이미지를 로드합니다
    with Redactor("./sample.jpg") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(er_opt)

        # 레드액션된 이미지를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg)를 클릭하세요.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

이 유형의 파일에 가리기를 적용할 수 없는 경우(예: BMP 이미지), [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/)는 [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/)가 됩니다.

## Redact embedded images

문서 내 모든 종류의 삽입 이미지에서 이미지 영역을 가릴 수 있습니다.

다음 예제는 Microsoft Word 문서 내 모든 삽입 이미지를 가리는 방법을 보여줍니다:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # 가릴 영역의 좌상단 위치를 정의합니다
    sample_point = Point(516, 311)
    # 가릴 영역의 크기를 정의합니다
    sample_size = Size(170, 35)
    # 레드액션 상자의 색상 정의
    color = Color.from_argb(255, 220, 20, 60)

    # 편집 옵션을 지정합니다
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 모든 삽입 이미지에 가리기를 적용합니다
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # 기본적으로 레드랙션된 문서는 PDF 형식으로 저장됩니다.
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx)를 클릭하세요.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

이 유형의 파일에 가리기를 적용할 수 없는 경우(예: 스프레드시트 문서), [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/)는 [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/)가 됩니다.

## Multi-frame images

주어진 원본과 프레임 수를 사용하여 다중 프레임 이미지에서 프레임을 제거할 수 있습니다. 추가 정보는 [remove page redactions]() 기사에서 확인하세요.

DjVu 문서와 같은 일부 이미지 형식은 [pre-rasterization]()이 필요하며 이후 PDF 형식으로 저장해야 합니다.
