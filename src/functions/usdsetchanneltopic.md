---
description: Sets a channel's topic
---

# $setChannelTopic

This function allows the bot to set a \<channel> topic

```
$setChannelTopic[channelID;new topic] ($setChannelTopc[channel id] will remove the topic)
```

Here's a simple usage

```javascript
bot.command({
name: "channel-topic".
code: `$setChannelTopic[$channelID;This is general chat!]`
})
```
