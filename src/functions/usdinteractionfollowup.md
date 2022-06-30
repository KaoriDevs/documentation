---
description: Following-up an deferred interaction message.
---

# $interactionFollowUp

`$interactionDefer`, defers the message for latest 15 minutes which can be used well for `$interactionFollowUp` function.

This function can be used for JSON requests, song informations or playing tracks, since these things takes more than 3 seconds.

### Usage

```php
$interactionFollowUp[content;embeds?;components?;files?;allowed mentions?]
```

### Fields

| Field            | Description                        | Required |
| ---------------- | ---------------------------------- | -------- |
| content          | A content message for reply        | no       |
| embeds           | Send embed messages for reply      | no       |
| components       | Adds components for reply          | no       |
| files            | Send file & attachment for reply   | no       |
| allowed mentions | Allowing to "x" mentions for reply | no       |

### Property Types

> * `CONTENT` — _classic message text 🤠_
> * `EMBEDS` — _embed-errors_
> * `COMPONENTS` — _buttons, selection menus_
> * `FILES` — _files & attachment embed-errors should be used in here._
> * `ALLOWED_MENTIONS` — _"USERS,ROLES,EVERYONE"_

**Footnotes**

* _If you want to make only embed message(s), you can just pass "content" property._
* Message can be ephemeral, if it's settled as `yes` on [$interactionDefer](functions/usdinteractiondefer.md)

## Example

This will make out interaction message as ephemeral message.

```javascript
bot.interactionCommand({
  name: "bye",
  prototype: 'slash',
  code: `
  $interactionFollowUp[Bye, world!]
  
  $interactionDefer[yes]
  `
});
```
