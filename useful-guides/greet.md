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

![Shortcut for greet](<../.gitbook/assets/image (3) (1).png>)

![Toggle by mentioning channel](<../.gitbook/assets/image (1) (1).png>)



Both methods will toggle greet on the channel. This means that, **if you type `a!greet` in a channel, greet will be enabled. Typing `a!greet` again will disable greet in that channel**

## Customizing Greet

You can view the current configurations of greet using the command `a!greet show`

![](<../.gitbook/assets/image (2) (1).png>)

### Changing the message

To change the current greet message, use the command `a!greet message <message>`

![Command to change greet message](<../.gitbook/assets/image (4).png>)

![Actual greet message](<../.gitbook/assets/image (5).png>)

You can use these variables in the message

| Placeholder      | Actual value                            |
| ---------------- | --------------------------------------- |
| `{mention}`      | The new member's mention (ping)         |
| `{mc}`           | The member count of the server          |
| `{server(name)}` | The name of the server                  |
| `{member(tag)}`  | The tag of the member (eg. Zapdos#0007) |
| `{member(name)}` | The username of the member (eg. Zapdos) |

### Setting delete after

Delete after is the number of seconds after which the greet message should be deleted. This can be helpful if you don't the channel to get flooded with greeting messages.

The command is `a!greet delafter <seconds>`

![To set delete after to 10 seconds](<../.gitbook/assets/image (2).png>)

{% hint style="info" %}
Set delete after to `0`, if you don't want messages to be deleted.

`a!greet delafter 0`
{% endhint %}



### That's it, you're done!

To review and test your final settings, you can click the :wrench:**Test Greet** button in `a!greet show`

