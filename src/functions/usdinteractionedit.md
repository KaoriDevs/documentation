---
description: Edit an interaction message.
---

# $interactionEdit

`$interactionEdit`, edits the interaction message send.

### Usage

```php
$interactionEdit[content;embeds?;components?;files?;allowed mentions?]
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
* Message _cannot_ be ephemeral, if it wasn't an ephemeral message before!

## Examples

```javascript
//Afte
bot.interactionCommand({
  name: "hello",
  prototype: 'slash',
  code: `
  $interactionEdit[Bye, World!]
  
  $wait[5s]
  
  $interactionReply[Hello, World!]
  `
});
```
