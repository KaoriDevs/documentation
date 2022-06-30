---
description: Returns the server name
---

# $serverName

This function returns the current/specified guild's name

```
$serverName[guild id (optional)]
```

```javascript
bot.command({
name: "serverName",
code: `Server Name: $serverName`
})
```
