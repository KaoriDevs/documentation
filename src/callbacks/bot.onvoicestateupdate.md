---
description: >-
  An event that gets executed, if the bot sees a user updating their voice
  status. To let the bot listen to the event, add one bot.onVoiceStateUpdate()
  callback inside your mainfile.
---

# bot.onVoiceStateUpdate

This callback triggers whenever someone joins a voice channel, leaves a voice channel or updates their vc options.

#### Usage:

```javascript
bot.voiceStateUpdateCommand({ //Command
channel: "id" // Log Channel
code: `code` //Your code
})
```

#### Example Command:

```javascript
bot.voiceStateUpdateCommand({ 
channel: "772414449839636490" 
code: `
$userTag[$newState[id]] has joined the vc $newState[channelName]
$onlyIf[$newState[channelID]!=;]
$onlyIf[$oldState[channelID]==;]
` 
})
```

#### Options:

You can use the functions $newState\[] and $oldState\[] with the options below to return old and new voice state data.

* `guildID` => The ID of the guild the voice state update happened in
* `guildName` => The name of the guild this voice state update happened
* `name` => The name of the user that updated its voice state
* `id` => The ID of the user that updated its voice state
* `channelID` => The ID of the voice channel this voice state update occurred in
* `channelName` => The name of the voice channel this voice state update occurred in
* `serverDeaf` => Whether the user is server deafened
* `selfDeaf` => Whether the user is self deafened
* `selfMute` => Whether the user is self muted
* `serverMute` => Whether the user is server muted
* `sessionID` => The ID of this voice session
* `streaming` => Whether this user is streaming
* `deaf`=> Whether the user is either self-deafened or server-deafened
* `mute` => Whether the user is either self-muted or server-muted
* `speaking` => Whether the user is speaking
