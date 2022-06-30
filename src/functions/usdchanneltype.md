---
description: Returns channel type
---

# $channelType

This function will show you the type of the specified channel.

### Usage

```php
$channelType[channelID?]
```

### Fields

| Field      | Description           | Type   | Required |
| ---------- | --------------------- | ------ | -------- |
| channel ID | The id of the channel | number | no       |

#### Types:

* `text` => normal text channel
* `voice` => voice channel
* `category` => category
* `news` => announcement channel
* `stage` => stage channel
* `dm` => dm channel
* `groupdm` => group dm channel
* `store` => store channel
* `newsthread` => thread in announcement channel
* `publicthread` => public thread channel
* `privatethread` => private thread channel

## Examples

* Get the channel type of the current channel:

```javascript
bot.command({
  name: "type",
  code: `The type of $channelName is $channelType`
});
```

* Get the channel type of the mentioned channel:

```javascript
bot.command({
  name: "type",
  code: `The type of $channelName[$mentionedChannels[1]] is $channelType[$mentionedChannels[1]]`
});
```
