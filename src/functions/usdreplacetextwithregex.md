# $replaceTextWithRegex

This function replaces text with [regex flags](https://www.w3schools.com/jsref/jsref\_obj\_regexp.asp)

```
$replaceTextWithRegex[text;regex;flags;new text]
```

```javascript
bot.command({
name: "regex",
code: `
$replaceTextWithRegex[hello aoi.js;aoi.js;g;community]
`
/*
Replaces 'aoi.js' to 'community'
*/
})
```
