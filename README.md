---
description: Here's how to setup Apollo for your server
---

# ⚙ Setup

### Add the bot to your server:

Use the following link to invite the bot to your server: [https://discord.com/api/oauth2/authorize?client\_id=824119071556763668\&permissions=8\&scope=applications.commands+bot](https://discord.com/api/oauth2/authorize?client\_id=824119071556763668\&permissions=8\&scope=applications.commands+bot)

{% embed url="https://dsc.gg/apollo-invite" %}
Invite Apollo
{% endembed %}

### Setup / FAQ

<details>

<summary>Greet (welcome message with ping)</summary>

Use the [`a!greet`](commands/page-1.md#greet) command to instantly start welcoming users without any extra setup.

Check out the [greet](commands/page-1.md) documentation to change the default settings.

</details>

<details>

<summary>Hosting giveaways </summary>

Use the [`a!gstart`](commands/giveaways.md#gstart) command to quickly start a giveaway.

You can create & assign a role called `Giveaways` to managers to give them access to create giveaways.

Check out the [giveaway](commands/giveaways.md) command documentation for more info.

</details>

<details>

<summary>Win message &#x26; claim time</summary>

1. Setup claim time using [claimtime](commands/claim-time.md#claimtime-add) command: `a!claimtime add everyone 10s`&#x20;
2. Using variables from [`a!variables`](commands/meta.md#variables), setup the win message using \[config] command: `a!config` -> Win message -> Set text win message
3. Use the \[config] command to enable the win message: `a!config` -> Win message -> Enable
4. If you're using other giveaway bots than Apollo, add triggers using the `a!config` command: `a!config` -> Triggers -> Add trigger
5. Make sure the giveaway winner has atleast one role with claimtime (assign `everyone` a claimtime to make sure)

You're all set!





</details>

<details>

<summary>Message counter</summary>

Use [`a!messages enable`](commands/message-counter.md#messages-enable) to instantly start counting messages.

Check out [message counter](commands/message-counter.md) for blacklisting/whitelisting channels or for adding/removing messages.

</details>



### More questions?

Join our support server & create a ticket so we can assist you!

{% embed url="https://discord.gg/apollo-hq-923425920096800788" %}
invite link to support server
{% endembed %}

