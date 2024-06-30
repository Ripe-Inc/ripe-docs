---
title: Managing Your Environment
layout: home
---
# Managing Your Environment

An environment has several properties you can use to customize your team's experience.

Name|Description
-|-
Endpoint|This is the main service API endpoint used to connect to your Ripe configuration environment
Private Keys|These are the keys intended to be used on backend servers and services to which the client should know nothing about
Public Keys|These are the keys intended to use in less secure locations such as mobile apps. These only expose the keys defined with the `Public` visibility.
Locked|This property prevents the environment from accepting any changes *outside* of a promotion
Limit Member Access|This property enables a dialog allowing you to define users as `Allow` or `Deny`. Users that are set to `Deny` cannot see anything about an environment, including keys, regardless of their role.
Restrict Network Access|This property enables a dialog allowing you to define ip addresses that are allowd to access this environments configuration through the endpoint. *Warning: Make sure that your ip addresses are accurate, as a mis-typed ip address will return 403 Forbidden*

## Rotating Keys
Keys can be rotated at whatever frequency you desire, buy pressing the `R` button to the right of a key. It is considered best practice to rotate keys regularly.

> [!WARNING]
>
> Rotating a key that is currently in use will immediately start returning 403 Forbidden from the service endpoint