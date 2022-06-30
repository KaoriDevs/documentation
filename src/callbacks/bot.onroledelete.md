---
description: >-
  An event that gets executed, if the bot sees a role deletion in one of it'S
  servers. To let the bot listen to the event, add one bot.onRoleDelete()
  callback inside your mainfile.
---

# bot.onRoleDelete

This callback triggers everytime a role gets deleted in a server.

#### Usage:

```javascript
bot.roleDeleteCommand({ //Command
channel: "channel ID", //Channel where its being logged
code: `your code` //Code sent to <channel>
})
```

#### Example Command:

```javascript
bot.roleDeleteCommand({ 
channel: "772414449839636490", 
code: `
Role Deleted:
Old Name: $oldRole[name]
`
})
```

#### Options:

You can use these functions [$oldRole\[\]](../functions/usdoldrole.md) with the options below to return old role data:

* `id` => The ID of the role
* `name` "The name of the role
* `position` => The position of this role
* `rawPosition` => The position of this role given by the API
* `hexColor` => The hex color for this role
* `color` => The color of this role
* `hoist` => Whether the role is hoisted or not
* `mentionable` => Whether the role is mentionable or not
* `guildID` => The ID of the guild the role belongs to
* `editable` => Whether the role is editable by the client or not
* `managed:` => Whether this role is managed by discord or not (bot- & booster-roles)
* `deleted:` => Whether the role was deleted or not
* `permissions` => The permissions for this role
