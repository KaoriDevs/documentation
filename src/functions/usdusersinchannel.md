---
description: >-
  Returns the users that are connected to the current voice channel that the bot
  is in.
---

# $usersInChannel

This function returns the users that are in the given voice channel.

### Usage

```php
$usersInChannel[voiceChannelID;option?;separator?]
```

### Fields

| Field          | Description                        | Type   | Required |
| -------------- | ---------------------------------- | ------ | -------- |
| voiceChannelID | The ID of the voice channel        | number | yes      |
| option?        | The option of the returning user's | string | no       |
| seperator?     | Seperator of userIDs               | string | no       |

#### Option Types

* `id` — Returns ID of the users with the given channel
* `user.username` — Returns name of the users with the given channel
* `nickname` — Returns nickname of the users with the given channel
* `mention` — Returns the users with mentioning from given channel

## Example

* Using this without given parameters

```javascript
bot.command({
  name: "users-in-channel",
  code: `
  $usersInChannel[$voiceID;nickname;, ]
  `
// Will return: Neo the Daddy, Kal'tsit
});
```
