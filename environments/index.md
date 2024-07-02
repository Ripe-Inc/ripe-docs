---
title: Environments
layout: home
nav_order: 5
has_children: true
---
# Environments

Environments in Ripe belong to Projects, and can have a specific value per key which is unique to the environment.

An environment has several properties you can use to customize your team's experience.

Name|Description
-|-
Endpoint|This is the main service API endpoint used to connect to your Ripe configuration environment
[Private Keys](api-keys)|These are the keys intended to be used on backend servers and services to which the client should know nothing about
[Public Keys](api-keys)|These are the keys intended to use in less secure locations such as mobile apps. These only expose the keys defined with the `Public` visibility.
Locked|This property prevents the environment from accepting any changes *outside* of a promotion
[Limit Member Access](limit-member-access)|This property enables a dialog allowing you to define users as `Allow` or `Deny`. Users that are set to `Deny` cannot see anything about an environment, including keys, regardless of their role.
[Restrict Network Access](network-access)|This property enables a dialog allowing you to define ip addresses that are allowd to access this environments configuration through the endpoint. *Warning: Make sure that your ip addresses are accurate, as a mis-typed ip address will return 403 Forbidden*
