---
description: Here's how to setup Apollo for your server
---

# ⚙ Setup

### Add the bot to your server:

{% embed url="https://dsc.gg/apollo-invite" %}
Invite Apollo
{% endembed %}

### Setup the commands:

<details>

<summary>Greet (welcome message with ping)</summary>

Use the `a!greet` command to instantly start welcoming users without any extra setup.

Check out the \[greet] documentation to change the default settings.

</details>

<details>

<summary>Hosting giveaways </summary>

Use the `a!gstart` command to quickly start a giveaway.

You can create & assign a role called `Giveaways` to managers to give them access to create giveaways.

Check out the \[giveaway] command documentation for more info.

</details>

<details>

<summary>Win message &#x26; claim time</summary>

1. Setup claim time using \[claimtime] command: `a!claimtime add everyone 10s`&#x20;
2. Using variables from `a!variables`, setup the win message using \[config] command: `a!config` -> Win message -> Set text win message
3. Use the \[config] command to enable the win message: `a!config` -> Win message -> Enable
4. If you're using other giveaway bots than Apollo, add triggers using the `a!config` command: `a!config` -> Triggers -> Add trigger
5. Make sure the giveaway winner has atleast one role with claimtime (assign `everyone` a claimtime to make sure)

You're all set!





</details>

<details>

<summary>Message counter</summary>

Use `a!messages enable` to instantly start counting messages.

Check out \[message counter] for blacklisting/whitelisting channels or for adding/removing messages.

</details>
