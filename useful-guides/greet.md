---
description: >-
  Guide for using the greeting feature in Apollo. Follow this to enable greet in
  your server.
---

# Greet

## Default Configurations

You don't need to set-up anything to enable greet. The default configurations are as follows:

Message: `{mention}, welcome to {server(name)}!`

Delete after: Each greeting message will be deleted after 5 seconds.

**You can go ahead with enabling greet without any configurations.**

## **Enabling Greet**

There are two ways to enable greet, all using the command `a!greet`.&#x20;

* Typing `a!greet` in the channel where you want greet to be enabled/disabled.
* Typing `a!greet #channel` will enable/disable greet in that channel.

![Shortcut for greet](<../.gitbook/assets/image (3).png>)

![Toggle by mentioning channel](<../.gitbook/assets/image (1).png>)



Both methods will toggle greet on the channel. This means that, **if you type `a!greet` in a channel, greet will be enabled. Typing `a!greet` again will disable greet in that channel**

## Customizing Greet

You can view the current configurations of greet using the command `a!greet show`

![](<../.gitbook/assets/image (2).png>)

### Changing the message

To change the current greet message, use the command `a!greet message <message>`

You can use these variables in the message

| Placeholder | Actual value                    |
| ----------- | ------------------------------- |
| `{mention}` | The new member's mention (ping) |
|             |                                 |
|             |                                 |
