---
description: Returns the server Icon
---

# $serverIcon

This function returns the current guild's icon

```
$serverIcon[guild ID (optional);size (optional);dynamic (optional)]
```

```javascript
bot.command({
name: "serverIcon",
code: `$thumbnail[$serverIcon]`
})
```
