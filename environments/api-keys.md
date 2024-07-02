---
title: Api Keys
layout: home
parent: Environments
---
# Api Keys

The Api keys found in your Environment Management dialog are used to access the Ripe environment through the service api `config.ripe.sh/...`. There are two sets of keys used for different purposes.

## Private Keys
These keys are intended for backend services, to which clients or third parties should not have access. These keys should be kept secret and you should rotate any keys you suspect might be leaked.

## Public Keys
These keys are intended for client facing apps such as mobile or web apps. These keys are intended to be less secure, and only expose the configurations in the `Public` visibility, regardless of if the configurations have been specified in the Api schema.

## Rotating Keys
Keys can be rotated at whatever frequency you desire, buy pressing the `R` button to the right of a key. It is considered best practice to rotate keys regularly.

{: .warning }
Rotating a key that is currently in use will immediately start returning 403 Forbidden from the service endpoint