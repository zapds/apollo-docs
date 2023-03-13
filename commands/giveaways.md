---
description: Commands for creating and controlling giveaways.
---

# Giveaways

## Controlling giveaways

### _**gstart**_

`a!gstart <time> <winners> <prize>`

Starts a new giveaway on the channel the command is run.

| Argument         | Description                                            | Example            |
| ---------------- | ------------------------------------------------------ | ------------------ |
| time (required)  | The duration of the giveaway in minutes, hours or days | 10m \| 2h \| 3d\|  |
| winners          | The number of winners to pick                          | 1w \| 2w \| 3w     |
| prize (required) | The prize for the giveaway.                            | Gift card \| Nitro |

### _**gend**_

`a!gend [message_id]`

Ends an ongoing giveaway forcefully.

| Argument               | Description                                                                                                                       | Example             |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------- |
| message\_id (optional) | The ID of the message containing the ongoing giveaway. If not provided, the command will choose the last giveaway in the channel. | 1084769011771920405 |

### _**greroll**_

`a!greroll [message_id]`

Chooses a new winner for an ended giveaway.

| Argument               | Description                                                                                                                     | Example             |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------- |
| message\_id (optional) | The ID of the message containing the ended giveaway. If not provided, the command will choose the last giveaway in the channel. | 1084769011771920405 |

## Managing giveaways

### _**glist**_

`a!glist`

Lists all giveaways of the server, to review/delete them.

### _**gdelete**_

`a!gdelete <message_id>`

Deletes a giveaway from the bot's database.

| Argument               | Description                                                  | Example             |
| ---------------------- | ------------------------------------------------------------ | ------------------- |
| message\_id (required) | The ID of the message containing the giveaway to be deleted. | 1084769011771920405 |

### _**gwblacklist**_

`a!gwblacklist [user]`

Blacklist/unblacklist a user from participating/winning all giveaways in the server. Providing a user will blacklist the user, while not providing a user will show the current blacklisted users.

| Argument | Description                                        | Example             |
| -------- | -------------------------------------------------- | ------------------- |
| user     | The user to blacklist. Leave empty to see the list | @user \| user#1234  |

## Other related commands

### _**wins**_

`a!wins [user]`

Shows the number of times a member won giveaways.

| Argument | Description                | Example            |
| -------- | -------------------------- | ------------------ |
| user     | The user to show wins for. | @user \| user#1234 |

### _**winrole**_

`a!winrole`

View current roles that are set to be added to giveaway winners.

### _**winrole set**_

`a!winrole set <role>`\
\
Adds a role to be added to the winner of a giveaway.

| Argument        | Description                    | Example              |
| --------------- | ------------------------------ | -------------------- |
| role (required) | The role to add to the winner. | @role \| 'role name' |
