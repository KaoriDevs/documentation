---
description: Clears all songs in queue besides 1st song in queue.
---

# $clearQueue

With this function you can clear the song queue completely but let the bot finish the current song before ending the music playback so queue will be purged but current song won't stop the playback.

### Usage

```php
$clearQueue
```

## Example

```javascript
bot.command({
name: "clear-queue",
code: `
I cleared the song queue and stop the music playback after the current song!
$clearQueue
`
})
```
