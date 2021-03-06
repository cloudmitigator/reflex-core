# reflex-core
## reflex
![Reflex](https://avatars3.githubusercontent.com/u/59374073?s=200&v=4)

Reflex enforces security best practices in cloud environments through event-driven automation. Get started by visiting [our documentation](https://docs.reflexivesecurity.com/).

## reflex-core
Package for the core Reflex classes. You can use these classes to easily create Reflex rules to secure your cloud environment (currently only supports AWS).

You'll also want to familiarize yourself with the other parts of Reflex:  
- [reflex-cli](https://www.github.com/reflexivesecurity/reflex-cli), a CLI for creating and managing your Reflex rules and environment.
- [reflex-engine](https://www.github.com/reflexivesecurity/reflex-engine), Terraform modules for deploying required Reflex rule infrastructure.
- [reflex documentation](https://docs.reflexivesecurity.com/), general documentation about deploying reflex.

## Installation
You can install `reflex-core` using `pip`.

`pip install reflex-core`

## Usage
To utilize `reflex-core`, simply import the rule class you want to utilize and implement the required methods.  

```
from reflex_core import AWSRule

class MyRule(AWSRule):
    def extract_event_data(event):
        # Logic for extracting required event info

    def resource_compliant():
        # Logic for determining if the resource configuration is compliant

    # etc
```

For examples, browse provided rules on [Reflexive Security's GitHub](https://www.github.com/reflexivesecurity/).

## License
Reflex is made available under the MPL 2.0 license. For more information view the [LICENSE](https://github.com/reflexivesecurity/reflex-core/blob/master/LICENSE)
