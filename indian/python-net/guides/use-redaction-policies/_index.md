---
title: "रेडैक्शन नीतियों का उपयोग करें"
linkTitle: "Use redaction policies"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "कैसे निपटना है सीखें। यदि आपके पास कॉरपोरेट संवेदनशील डेटा हटाने की नीति रेडैक्शन नियमों की सूची के रूप में है, तो आपको उन्हें कोड में निर्दिष्ट करने की आवश्यकता नहीं है। आप प्री‑कॉन्फ़िगर किए गए रेडैक्शन की सूची के साथ एक XML दस्तावेज़ निर्दिष्ट कर सकते हैं।"
type: docs
url: /hi/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


यदि आपके पास कॉरपोरेट संवेदनशील डेटा हटाने की नीति रेडैक्शन नियमों की सूची के रूप में है, तो आपको उन्हें कोड में निर्दिष्ट करने की आवश्यकता नहीं है। आप प्री‑कॉन्फ़िगर किए गए रेडैक्शन की सूची के साथ एक XML दस्तावेज़ निर्दिष्ट कर सकते हैं।

नीचे रेडैक्शन नीति XML फ़ाइल का एक उदाहरण दिया गया है (कोड प्रॉपर्टीज़ मैपिंग स्पष्ट है):

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
आप `RedactionPolicy.save()` मेथड का उपयोग करके इस संरचना की XML दस्तावेज़ बना सकते हैं, रनटाइम में रेडैक्शन को कॉन्फ़िगर करते हुए।

निम्न उदाहरण दर्शाता है कि कैसे एक [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) को XML फ़ाइल में सहेजा जाए।
 

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
    # रेडैक्शन का रंग निर्धारित करें
    color = Color.from_argb(255, 220, 20, 60)

    # रेडैक्शन को कॉन्फ़िगर करें
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # नीति बनाएं
    policy = RedactionPolicy(redactions)

    # रेडैक्शन नीति को XML फ़ाइल में सहेजें
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

आप जितनी भी नीतियाँ चाहें बना सकते हैं, उन्हें लोड करके अपने दस्तावेज़ों को रेडैक्ट कर सकते हैं।

नीचे दिया गया उदाहरण XML फ़ाइल से एक रेडैक्शन नीति लोड करता है और इसमें मौजूद प्रत्येक नियम को एक दस्तावेज़ पर एकल `apply` कॉल में लागू करता है:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # XML फ़ाइल से रेडैक्शन नीति लोड करें
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # दस्तावेज़ लोड करें और एक कॉल में पूरी नीति लागू करें
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # मूल स्वरूप बनाए रखें और आउटपुट नाम में एक प्रत्यय जोड़ें
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` इस उदाहरण में उपयोग की गई नीति फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) क्लिक करें।

`sample.docx` इस उदाहरण में रेडैक्ट किया गया दस्तावेज़ है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) क्लिक करें।

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)
