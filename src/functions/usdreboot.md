# $reboot

This function technically allows you a restart the bot, or a file

```
$reboot[path]
```

Using the function

```javascript
bot.command({
name: "reboot",
code: `$reboot[server.js]`,
}) //server.js aka our main file, this will restart the bot
```
