# $archiveThread

This function used for archiving an active thread.

### Usage

```php
$archiveThread[threadID;channelID;archive?;reason?]
```

### Fields

| Field     | Description                      | Type   | Required |
| --------- | -------------------------------- | ------ | -------- |
| threadID  | The ID of the thread             | number | yes      |
| channelID | The ID of the channel            | number | yes      |
| archiving | Archiving or making active.      | string | no       |
| reason    | Reason for archiving/activating. | string | no       |

## Examples

* Archiving a thread:

```javascript
bot.command({
    name: "archive-thread",
    code: `
    $archiveThread[938078671095365693;722031482163560499;yes;Thanks for talk!]
    `
});
```

* Activating a thread:

```javascript
bot.command({
    name: "active-thread",
    code: `
    $archiveThread[938078671095365693;722031482163560499;no;Let's talk again!]
    `
});
```
