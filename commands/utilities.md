---
description: Category of unique and useful commands you can use.
---

# Utilities

{% hint style="info" %}
_<mark style="color:blue;">**Reading the documentation**</mark>_

`<argument>` - Required

`[argument]` - Optional

<mark style="color:red;">**Do NOT type <> or \[] when using the commands.**</mark>
{% endhint %}



All prefixes in the documentation are given as `a!`, which is the default prefix. Prefixes are changeable per server, so mention @Apollo to get the prefix for the server.

###

### User Utilities

| Command                     | Information                                                                                                                                                                                         |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `a!snipe [channel] [index]` | Shows the last deleted message. You can specify an optional channel to get the deleted messages from that channel. Index should be a number from 1 - 10, 1 being the most recent message deleted.   |
| `a!snipetoggle`             | Toggles allowing others to snipe your messages.                                                                                                                                                     |
| `a!afk [reason]`            | Marks the user ask AFK, until a new message is sent. While AFK, all members who mention the user are replied with a reason why the user is AFK.                                                     |
| `a!avatar [user]`           | Shows the avatar and banner of a specified user. Defaults to the author.                                                                                                                            |

### Guild Utilities

| Command                      | Information                                                                                                                                                         |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `a!purge [user] <value>`     | Deletes a certain number of messages. If a user is specified, messages sent by the user are only deleted. Value is the number of messages to search for, to delete. |
| `a!purge bots <amount>`      | Deletes messages sent by bots.                                                                                                                                      |
| `a!purge images <amount>`    | Deletes messages containing attachments.                                                                                                                            |
| `a!purge humans <amount>`    | Deletes messages sent by users (not bots).                                                                                                                          |
| `a!purge embeds <amount>`    | Deletes messages containing embeds.                                                                                                                                 |
| `a!greet [channels]`         | Toggles greet on the channels, or the channel in which the command is run. While greet is active, new members are welcomed with a message.                          |
| `a!greet message <message>`  | Sets the welcome message for greet.                                                                                                                                 |
| `a!greet delafter <seconds>` | Sets the number of seconds after which the welcome message should be deleted. Setting seconds to `0` will **not** delete the welcome message.                       |
| `a!greet show`               | Shows the configuration of greet.                                                                                                                                   |
| `a!embed`                    | Creates a new embed, which is fully customizable. You can also set the embed to be sent in a specific channel, or set it as the win message.                        |
| `a!timestamp <time>`         | Gives you the Discord-formatted timestamp for the given time.                                                                                                       |
| `a!timedif <ID_1> [ID_2]`    | Shows the time difference between two discord IDs. Check out [how-to-use-timedif.md](../guides/how-to-use-timedif.md "mention") to learn more.                      |

### Server Utilities

| Command                                  | Information                                                          |
| ---------------------------------------- | -------------------------------------------------------------------- |
| `a!movech <category_id> <channel_id>`    | Moves a Channel To Another Category.                                 |
| `a!roleicon <emoji_id> [or] <image_url>` | Sets An Emoji As The Role Icon. \[Works If Your Server Has 7 Boosts] |
| `a!nuke <channel>`                       | Clones The Channel So Pings Are Removed.                             |
| `a!newrole`                              | Creates a New Role Of Your Choice.                                   |
| `a!userinfo <user>`                      | Shows Information About a User.                                      |

