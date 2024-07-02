---
title: Member Access
layout: home
parent: Environments
---
# Member Access

In an Enviornment, you can limit the member access to only specific members in your team. This is useful in situations where you want to segregate different departments/responsabilities between different environments, or maybe you'd like to prevent users from seeing production configurations.

You can modify the member access in the Environment Settings dialog, by pressing the gear icon next to Environments in the navigation menu.

First, you must enable the `Limit Member Access` option in the environment settings. This will display a button which opens the Member Access dialog.

![Limit member access button](../img/proj-limit-members-2.png "Limit member access button")

From the Manage Member Access dialog you can set specific members to `Allow` or `Deny` based off of your preferences. 

![Limit member access dialog](../img/proj-limit-members-3.png "Limit member access dialog")

{: .new }
Once you've made your changes to this dialog, close it by pressing the `x` in the top right corner of the dialog. Then you must Save the environment for the changes to take effect.

{: .warning }
Once you enable the `Limit Member Access` checkbox in a environment, users who are set to `Deny` will no longer access any of the content in the environment, regardless or their role.