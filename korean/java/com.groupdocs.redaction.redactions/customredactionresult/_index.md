---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "결과를 반환함을 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

결과를 반환함을 나타냅니다 [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getApply()](#getApply--) | 교체가 적용되어야 하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | 교체가 적용되어야 하는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getText()](#getText--) | 교체가 #getApply().getApply()인 경우 사용되는 교체 텍스트를 가져옵니다 |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | 교체가 #getApply().getApply()인 경우 사용되는 교체 텍스트를 설정합니다 |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


교체가 적용되어야 하는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean -  true  일치하는 텍스트를 #getText().getText()로 교체하려면; 그렇지 않으면,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


교체가 적용되어야 하는지 여부를 나타내는 값을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | true  교체를 적용하려면; 그렇지 않으면,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


교체가 #getApply().getApply()인 경우 사용되는 교체 텍스트를 가져옵니다
true
.


**Returns:**
java.lang.String - 교체 텍스트.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


교체가 #getApply().getApply()인 경우 사용되는 교체 텍스트를 설정합니다
true
.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 대체 텍스트. |
|

