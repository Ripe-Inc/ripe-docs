---
title: Network Access
layout: home
parent: Environments
---
# Network Access

In an environment you can limit the network access to your configuration endpoint. Enabling this setting will block access to the configuration endpoint unless it comes from a specific IP Address.

You can enable this by navigating to the Environment Management dialog by clicking the gear icon next to Environments in the navigation bar. Enable `Restrict Network Access` and use the `Manage Network Access` button to configure.

![Manage Network Access](../img/env-network-access-1.png "Manage Network Access")

The dialog will now be visible

![Manage Network Access](../img/env-network-access-2.png "Manage Network Access")

You can configure a specific IP Address, an IP Address range by clicking the `Range` checkbox, or use an IP Address with the wildcard operator. 

{: .note }
You can save by pressing the `x` in the top corner of the dialog, and then saving the environment. You must save the environment for the changes to take effect.

{: .warning }
Once you save the environment, any IP Addresses that don't match while `Restrict Network Access` is on will return a 403 Forbidden when accessing the environment endpoint!