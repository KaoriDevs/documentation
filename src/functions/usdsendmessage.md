---
description: Sends a message to the current channel
---

# $sendMessage

This function sends the \<message> to the current channel

```
$sendMessage[message;return message ID (yes/no)(required)]
```

```javascript
bot.command({
name: "sendMessage",
code: `$sendMessage[aoi.js is awesome;no]
//this will not send the message ID`
})
```
