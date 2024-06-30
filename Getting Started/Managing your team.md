# Managing Your Team

You can manage your team in Ripe if your role access is either `Owner` or `Administrator`. The following roles can be assigned to users in your team through the `Settings -> Manage Team` menu:

Role Name|Description
-|-
Read Only|This is the default role for users, and allows them to read but not modify and data
Read Write|This role allows users to make key edits and create keys and create promotions
Manager|This role is similar to Read Write, but also allows the user to manage Projects/Environments, as well as approve promotions
Administrator|This role allows users to create Projects/Environments and assign other users different roles
Billing|This role is unique in that its similar to Read Only, but with the added benefit of managing billing subscription details for the team
Owner|This is the creator of the team, and has all the access

An additional aspect to managing a team is monitering the Quota. Users with the `Owner`, `Administrator` or `Billing` role can view the Quota through the `Settings -> Manage Team` menu:

Name|Description
-|-
Service Calls|This is the current/maximum number of service and API calls your team can accept per day
Members|This is the maximum number of members your team can have
Projects|This is the maximum number of Projects your team can have
Environments|This is the maximum number of Environments your team can have
Log Retention|This is the maximum number of days that logs are stored for your team. Logs include service and API request logs, and the logs regarding any change to keys, environments, projects, and users.