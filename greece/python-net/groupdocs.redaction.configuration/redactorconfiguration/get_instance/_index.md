---
title: "Μέθοδος get_instance"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Επιστρέφει ένα μοναδικό (singleton) αντικείμενο με την προεπιλεγμένη ρύθμιση των ενσωματωμένων μορφών."
type: docs
url: /el/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Επιστρέφει ένα μοναδικό (singleton) αντικείμενο με την προεπιλεγμένη ρύθμιση των ενσωματωμένων μορφών.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Παράδειγμα

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Αποκτήστε τη singleton διαμόρφωση
config = RedactorConfiguration.get_instance()

# Επεκτείνετε τις υποστηριζόμενες επεκτάσεις για μορφές απλού κειμένου
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### Δείτε επίσης
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
