---
title: Anatomy of a Key
layout: home
---
# Anatomy of a Key

Keys are what makes Ripe work. A Key has several properties that we're going to go over now.

## Names
A key must have a name, and that name may contain characters `a-Z`, `0-9`, `.`, `-` and `_`.

A Key's name must be unique to a project, regardless of casing. Some edge case duplicate keys:
```
My.Test.Key
my.test //This key is a duplicate because the section above has reserved the name
```

The period is used to express sections in a key name. The following example shows this in action for the key `My.Test.Bool` and `My.Test.String`:
```json
"My":{
    "Test":{
        "Bool":"",
        "String":""
    }
}
```

## Value Type
A key must have a **Value Type** this is a type constraint on the key, allowing you to safely assume a key will always be a specific type. Here is a list of the current types and their default values
Type|Default
-|-
String|` `
Boolean|`false`
Integer|`0`
Decimal|`0`
JSON|`{}`

> [!IMPORTANT]
> 
> This assumes the key you're requesting exists in the project you're requesting against. Any key that does not exist when making the request will return null.

## Key Visibility
When creating and editing a key its important to remember the visibility of the key. A key can be either `Public` or `Private`, and this visibility cannot be changed later without deleting the key. 

This visibility separation allows you to use a specific set of keys in places other than a background server, such as in a mobile app. This way you can keep sensitive and non-sensitive data in the same environment.

## Key : Project : Environment Relationship
A Key belongs in a Project, which can have many keys. When creating a key, every environment is automatically assigned the default **Value**

A **Value** can be assigned to an Environment *for* a key. Every environment can have one value for one key. This means that configurations between Environments can have completely different values, but will always have the same keys within the Project.

## Optional Key Properties

* **Description**: This allows you to add context to what the key is for. This property can be modified after creation, and does not change between environments.
* **Tags**: Tags can be created for a project and assigned to a key. This property can be modified after creation, and does not change between environments.
* **Value**: A value can be assigned to a key *per* environment. This can be modified after creation.
* **Rules**: A key can have several rules to return a specific value based on select criteria. Rules are unique per environment.
* **Is Sticky**: A key can be set as `Is Sticky` this an environment specific property, that when true, prevents promotions from overriding the value. This property can help reduce noise generated in promotions for values that never change.