---
description: Customizing Apollo to get started with the bot.
---

# Configurations

{% hint style="warning" %}
_<mark style="color:orange;">**Apollo will NOT work unless set up.**</mark>_

Setting up the configurations is required for Apollo to send win message.
{% endhint %}

The main command for configurations is `a!config`. All settings for the server can be managed using this command.



## Basic Setup

Use the command `a!quicksetup` to apply the basic settings for the server. It will:

* Add GiveawayBot triggers like g!end and g!reroll.
* Set a default win message.
* Add claim time of 10 seconds to everyone.

You can change these settings any time, using the `a!config` command.

{% hint style="success" %}
<mark style="color:green;">**You don't need to add Apollo's giveaway triggers.**</mark>

As long as win message is enabled, win message will be sent in Apollo's giveaways. You don't need to add triggers like `a!greroll` or `a!gend`
{% endhint %}



## Customizing Apollo

### Adding claim time

Use the command `a!claimtime add` to add claim time to roles.

Example: `a!claimtime add @role 5s` will add 5 seconds to the role.&#x20;

The command `a!claimtime remove @role` can be used to delete claim time of a role.

{% hint style="info" %}
<mark style="color:blue;">**Override**</mark>

If override is enabled and the claim time for the role is 10 seconds, then everyone with the role will get ONLY 10 seconds to claim. If override is disabled, Apollo will add 10 seconds to other claim times to get the total claim time.
{% endhint %}
