---
description: Commands that provide utility
---

# Utilities

### _**timer**_

`a!timer <duration> [name]`

Set a timer that will end after the specified duration. The timer can be given a name to help identify it when it ends.

| Argument            | Description                                    | Example            |
| ------------------- | ---------------------------------------------- | ------------------ |
| duration (required) | The duration of the timer in minutes or hours. | 10m \| 2h \| 3h30m |
| name                | The name of the timer.                         | Event end          |

### _**timestamp**_

`a!timestamp <time>`

Gives you the Discord-formatted timestamp for a time. The time can be specified in various formats, such as `2d`, `3w`, `in 3 days`, `14/03/23`, or `last week`.

| Argument        | Description                           | Example                                                  |
| --------------- | ------------------------------------- | -------------------------------------------------------- |
| time (required) | The time to generate a timestamp for. | `2d` \| `3w` \| `in 3 days` \| `14/03/23` \| `last week` |

### _**movech**_

`a!movech <category>`

Moves a text channel to a selected category, provided its mention or ID.

| Argument            | Description                                               | Example                    |
| ------------------- | --------------------------------------------------------- | -------------------------- |
| category (required) | The mention or ID of the category to move the channel to. | `#general` \| `1234567890` |



### _**roleicon**_

`a!roleicon <role> <emoji>`

Edits a role to set an emoji as its icon. Only custom emojis are supported.

| Argument         | Description                         | Example                      |
| ---------------- | ----------------------------------- | ---------------------------- |
| role (required)  | The role to set the emoji icon for. | `@moderator` \| `1234567890` |
| emoji (required) | The emoji to use as the role icon.  | `:customemoji:`              |

### _**snipe**_

`a!snipe [channel] [index]`

Gets the last deleted message(s) in the channel. The index can be a number from 0 to 10 or can be `all` to get all 10 deleted messages.

| Argument           | Description                                                                                                                                                                   | Example                    |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
| channel (optional) | The channel to get the deleted messages from. If not provided, the current channel will be used.                                                                              | `#general` \| `1234567890` |
| index (optional)   | The index of the deleted message to retrieve. If not provided, the most recent deleted message will be retrieved. If set to `all`, all 10 deleted messages will be retrieved. | `3` \| `all`               |

### _**snipetoggle**_

`a!snipetoggle`

Toggles between allowing other users to view the author's deleted messages.

### _**purge**_

`a!purge <amount> [options]...`

Deletes messages in bulk. Ignores pinned messages. You can specify options to filter the messages to delete. Options available are:

* `bots` Deletes messages sent by bots.
* `humans` Deletes messages sent by humans.
* `embeds` Deletes messages that contain embeds.
* `attachments` Deletes messages that contain attachments.

Multiple options can also be specified.

| Argument           | Description                                                          | Example                        |
| ------------------ | -------------------------------------------------------------------- | ------------------------------ |
| amount (required)  | The number of messages to delete. The limit is 100 messages at once. | `50`                           |
| options (optional) | The filtering options to use when deleting messages.                 | `bots` \| `embeds attachments` |

### _**nuke**_

`a!nuke [channel]`

Clones a channel, and then deletes the original. This can be used for removing unwanted pings or for deleting all messages in the channel.

| Argument           | Description                                                              | Example                    |
| ------------------ | ------------------------------------------------------------------------ | -------------------------- |
| channel (optional) | The channel to nuke. If not provided, the current channel will be nuked. | `#general` \| `1234567890` |

### _**clone**_

`a!clone [channel]`

Copies a channel's name and permissions and creates a new one.

| Argument           | Description                                                                | Example                    |
| ------------------ | -------------------------------------------------------------------------- | -------------------------- |
| channel (optional) | The channel to clone. If not provided, the current channel will be cloned. | `#general` \| `1234567890` |

### _**timedif**_

`a!timedif <message_id_1> [message_id_2]`

Shows the difference between to discord objects. This can be used to check time intervals of two messages. You can use this command in two ways:

* Specifying both message IDs `a!timedif 1234567890 1234567890`
* Specifying one message ID, while replying to the other `a!timedif 123456789`

| Argument                  | Description                                                                  | Example              |
| ------------------------- | ---------------------------------------------------------------------------- | -------------------- |
| message\_id\_1 (required) | The first message ID to compare.                                             | `123456789012345678` |
| message\_id\_2            | The second message ID to compare. If using the reply method, leave it blank. | `123456789012345678` |

### _**avatar**_

`a!avatar [member]`

Shows a user's avatar, banner, accent colour and other assets. If member is not specified, shows information for the user who issued the command.

| Argument          | Description                      | Example                              |
| ----------------- | -------------------------------- | ------------------------------------ |
| member (optional) | The member whose assets to show. | `@user#1234` \| `123456789012345678` |

### _**userinfo**_

`a!userinfo [member]`

Shows all available information about the user. If member is not specified, shows information for the user who issued the command.

| Argument          | Description                           | Example                              |
| ----------------- | ------------------------------------- | ------------------------------------ |
| member (optional) | The member whose information to show. | `@user#1234` \| `123456789012345678` |

### _**afk**_

`a!afk [all_servers] [reason]`

Marks the author as AFK. While AFK, the bot will reply to all user pings & record them.

| Argument                | Description                                   | Example            |
| ----------------------- | --------------------------------------------- | ------------------ |
| all\_servers (optional) | Whether the user is going AFK in all servers. | `true` \| `false`  |
| reason (optional)       | The reason why the user is going AFK.         | `out for vacation` |

### _**membercount**_

`a!membercount`

Shows the number of total members in the server.

### _**serverinfo**_

`a!serverinfo`

Shows detailed information about the server.

### _**embed**_

`a!embed [json]`

Easily construct fully customizable Discord embeds. You can import an embed by:

* Replying to a message with an embed
* Providing the JSON as an argument
* Attaching a JSON file with the message

| Argument | Description           | Example                                      |
| -------- | --------------------- | -------------------------------------------- |
| json     | The JSON of the embed | `{"title": "Hello", "description": "World"}` |

### _translate_

Translates a given text or the replied message's content to another language.

<details>

<summary>Language codes</summary>

`af`-Afrikaans, `sq`-Albanian, `am`-Amharic, `ar`-Arabic, `hy`-Armenian, `az`-Azerbaijani, `eu`-Basque, `be`-Belarusian, `bn`-Bengali, `bs`-Bosnian, `bg`-Bulgarian, `ca`-Catalan, `ceb`-Cebuano, `ny`-Chichewa, `zh-cn`-Chinese (simplified), `zh-tw`-Chinese (traditional), `co`-Corsican, `hr`-Croatian, `cs`-Czech, `da`-Danish, `nl`-Dutch, `en`-English, `eo`-Esperanto, `et`-Estonian, `tl`-Filipino, `fi`-Finnish, `fr`-French, `fy`-Frisian, `gl`-Galician, `ka`-Georgian, `de`-German, `el`-Greek, `gu`-Gujarati, `ht`-Haitian creole, `ha`-Hausa, `haw`-Hawaiian, `iw`-Hebrew, `he`-Hebrew, `hi`-Hindi, `hmn`-Hmong, `hu`-Hungarian, `is`-Icelandic, `ig`-Igbo, `id`-Indonesian, `ga`-Irish, `it`-Italian, `ja`-Japanese, `jw`-Javanese, `kn`-Kannada, `kk`-Kazakh, `km`-Khmer, `ko`-Korean, `ku`-Kurdish (kurmanji), `ky`-Kyrgyz, `lo`-Lao, `la`-Latin, `lv`-Latvian, `lt`-Lithuanian, `lb`-Luxembourgish, `mk`-Macedonian, `mg`-Malagasy, `ms`-Malay, `ml`-Malayalam, `mt`-Maltese, `mi`-Maori, `mr`-Marathi, `mn`-Mongolian, `my`-Myanmar (burmese), `ne`-Nepali, `no`-Norwegian, `or`-Odia, `ps`-Pashto, `fa`-Persian, `pl`-Polish, `pt`-Portuguese, `pa`-Punjabi, `ro`-Romanian, `ru`-Russian, `sm`-Samoan, `gd`-Scots gaelic, `sr`-Serbian, `st`-Sesotho, `sn`-Shona, `sd`-Sindhi, `si`-Sinhala, `sk`-Slovak, `sl`-Slovenian, `so`-Somali, `es`-Spanish, `su`-Sundanese, `sw`-Swahili, `sv`-Swedish, `tg`-Tajik, `ta`-Tamil, `te`-Telugu, `th`-Thai, `tr`-Turkish, `uk`-Ukrainian, `ur`-Urdu, `ug`-Uyghur, `uz`-Uzbek, `vi`-Vietnamese, `cy`-Welsh, `xh`-Xhosa, `yi`-Yiddish, `yo`-Yoruba, `zu`-Zulu

</details>

| Argument          | Description                              | Example       |
| ----------------- | ---------------------------------------- | ------------- |
| destination\_lang | The destination language to translate to | `es` \| `fr`  |
| text              | The text to translate.                   | Hola          |

### _**rename**_

`a!rename [channel] <name>`

Edits the given channel's name to the name given.

| Argument           | Description                                                      | Example  |
| ------------------ | ---------------------------------------------------------------- | -------- |
| channel (optional) | The channel to rename. If not provided, defaults to current one. | #general |
| name (required)    | The new name for the channel.                                    | new name |
