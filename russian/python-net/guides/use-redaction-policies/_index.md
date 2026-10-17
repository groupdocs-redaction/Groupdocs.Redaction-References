---
title: "Используйте политики редактирования"
linkTitle: "Use redaction policies"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Узнайте, как действовать. Если у вас есть корпоративная политика удаления конфиденциальных данных в виде списка правил редактирования, вам не нужно указывать их в коде. Вы можете задать XML‑документ со списком преднастроенных редактирований."
type: docs
url: /ru/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Если у вас есть корпоративная политика удаления конфиденциальных данных в виде списка правил редактирования, вам не нужно указывать их в коде. Вы можете задать XML‑документ со списком преднастроенных редактирований.

Ниже приведён пример XML‑файла политики редактирования (соответствие свойств кода очевидно):

**RedactionPolicy.xml**

```xml
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns="http://www.groupdocs.com/redaction">  
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase="dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <eraseMetadataRedaction filter="All" />  
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
  <annotationRedaction regularExpression="(anno1)" replacement="foobar" />  
  <deleteAnnotationRedaction regularExpression="(anno2)" />  
  
  <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
  <imageAreaRedaction pointX="110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy> 
```
Вы можете использовать метод RedactionPolicy.save() для создания XML‑документов такой структуры, настраивая редактирование во время выполнения.

Следующий пример демонстрирует, как сохранить [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) в XML‑файл.
 

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    ReplacementOptions,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def create_redaction_policy():
    # Определите цвет редактирования
    color = Color.from_argb(255, 220, 20, 60)

    # Настройте редактирование
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Создайте политику
    policy = RedactionPolicy(redactions)

    # Сохраните политику редактирования в XML‑файл
    policy.save("./sample_policy.xml")
    print("Redactions policy saved to ./sample_policy.xml")

if __name__ == "__main__":
    create_redaction_policy()
```

  
```text
<?xml version="1.0"?>
<redactionPolicy>
  <exactPhraseRedaction actionType="ReplaceString" replacement="[Product]" searchPhrase="Redaction" />
  <regexRedaction actionType="DrawBox" color="#DC143C" regularExpression="\d{2}\s*\d{2}[^\d]*\d{6}" />
  <deleteAnnotationRedaction regularExpression="[.]*" />
  <eraseMetadataRedaction filter="All" />
</redactionPolicy>
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/create_redaction_policy/sample_policy.xml)

Вы можете создать столько политик, сколько потребуется, загружая их для редактирования ваших документов.

Пример ниже загружает политику редактирования из XML‑файла и применяет каждое правило, которое она содержит, к документу одним вызовом `apply`:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Загрузите политику редактирования из XML‑файла
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Загрузите документ и примените всю политику одним вызовом
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Сохраните оригинальный формат и добавьте суффикс к имени выходного файла
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` — файл политики, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) чтобы скачать его.

`sample.docx` — документ, подвергнутый редактированию в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) чтобы скачать его.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)
