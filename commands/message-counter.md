---
description: Commands to count messages.
---

# Message Counter

{% hint style="info" %}
Check the [`a!messages settings`](message-counter.md#messages-settings) command to blacklist/whitelist channels where messages should be counted.
{% endhint %}

### _**messages**_

`a!messages [user]`

Shows the number of messages a member has sent.

| Argument | Description                         | Example            |
| -------- | ----------------------------------- | ------------------ |
| user     | The user to show message count for. | @user \| user#1234 |

### _**messages enable**_

`a!messages enable`

Enables the counting of messages for the server.

### _**messages disable**_

`a!messages disable`

Disables the counting of messages for the server.

### _**messages add**_

`a!messages add <member> <amount>`

Adds a certain number of messages to a member's message count.

| Argument | Description                                  | Example            |
| -------- | -------------------------------------------- | ------------------ |
| member   | The member to add messages to.               | @user \| user#1234 |
| amount   | The number of messages to add to the member. | 100                |

### _**messages remove**_

`a!messages remove <member> <amount>`

Remove a certain number of messages to a member's message count.

| Argument | Description                                       | Example            |
| -------- | ------------------------------------------------- | ------------------ |
| member   | The member to remove messages from.               | @user \| user#1234 |
| amount   | The number of messages to remove from the member. | 100                |

### _**messages reset**_

`a!messages reset [member]`

Resets a member's or the whole server's message count to 0.

| Argument | Description                                                                 | Example            |
| -------- | --------------------------------------------------------------------------- | ------------------ |
| member   | The member to reset message count for. If not provided, resets server-wide. | @user \| user#1234 |

### _**messages settings**_

`a!messages settings`

Displays all settings related to message counting in the server.

Settings available:

* Blacklist mode: Don't count messages from selected channels
* Whitelist mode: Only count messages from selected channels
* All channels: Count messages from all channels (default)

