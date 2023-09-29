---
description: Greet system to welcome new members.
---

# Greeter

{% hint style="info" %}
Variables\
\
To ping the user, use `{mention}`\
To show server name, use `{server(name)}`\
To show member count, use `{mc}`&#x20;

See the `a!variables` command to view a full list of these variables
{% endhint %}

### _**greet**_

`a!greet [channel]`

Toggles greet in the specified channel. It will enable greet if it's disabled, or disable it if enabled.

| Argument | Description                                                         | Example        |
| -------- | ------------------------------------------------------------------- | -------------- |
| channel  | The channel to enable/disable greet. If not provided, uses current. | #channel-name  |

### _**greet show**_

`a!greet show`

Shows the configurations of greet.

### _**greet message**_

`a!greet message <message>`

Sets the message to be sent when a member joins.

| Argument | Description                               | Example                          |
| -------- | ----------------------------------------- | -------------------------------- |
| message  | The message to be sent when member joins. | Welcome to the server, {mention} |

### _**greet delafter**_

`a!greet delafter <seconds>`

Sets the time to delete the greet message after a member joins.

| Argument | Description                                                        | Example |
| -------- | ------------------------------------------------------------------ | ------- |
| seconds  | The time in seconds after which the greet message will be deleted. | 5       |

### Greet Message Variables

These are special keywords that will be replaced with their actual value.

| Variable       | Value                     | Example   |
| -------------- | ------------------------- | --------- |
| {mention}      | The member's mention      | @Zapdos   |
| {mc}           | The server's member count | 1         |
| {server(name)} | The server's name         | Apollo HQ |
| {member(tag)}  | The member's username     | zapd0s.   |
| {member(name)} | The member's name         | zapd0s.   |
