---
title: DocumentFormatInstance class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a specific format of a document and can be implemented to add custom document types."
type: docs
url: /python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Represents a specific format of a document and can be implemented to add custom document types.

Learn more

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

The DocumentFormatInstance type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Initializes the document format handler instance. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Checks for [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) implementation and invokes it, if specified. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Loads the document from a stream. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Checks if the given stream contains a document supported by this format instance. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Saves the document to a stream. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Properties
| Property | Description |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | The password for password-protected documents. |

### Example

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # load file content
        pass

    def save(self, output: io.RawIOBase) -> None:
        # save changes to file
        pass
```

```python
class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        self.my_property = None

    def initialize(self, config: DocumentFormatConfiguration) -> None:
        super().initialize(config)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]
```

### See Also
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
