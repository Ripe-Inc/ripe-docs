---
title: Raw Data
layout: home
nav_order: 8
---
# Raw Data

The Raw Data section of your environment can be found in the top bar of the environment. This dialog allows you to view the current environment in JSON format, as well as a few other formats.

## Flat JSON
The Flat JSON view flattens your environment into a single object using either `.` or `:` to separate sections. There is also an edit button in the top right of the JSON editor that allows you to modify values quickly.

{: .warning }
Modifying values this way is dangerous! Only values can be modified in this view; any key changes will be discarded. Trying to change value type will invalidate the save

## Keys
The keys section allow you to see the information on all the keys in your project. There is an edit button in the top right of the JSON editor that allows you to modify keys quickly

{: .warning }
Modifying keys this way is dangerous and destructive! Any changes made here can be unpredictable and have implications across the entire project. This should only be used for migrating a project to another project quickly.