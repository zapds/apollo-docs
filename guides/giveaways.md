---
description: In this page, you will learn about hosting & managing giveaways using Apollo.
cover: ../.gitbook/assets/covergradient-5.png
coverY: 0
---

# Giveaways

As you know apollo has a very sophisticated and advanced giveaway system. This page will walk through each and every command in detail so you can use the most out of apollo giveaway system.

## Giveaway Management Commands

### a!wins

> This command shows the amount of win counts of giveaways hosted in the particular server and in all the servers apollo is in. In addition to the count, this command also shows what prize has been won by that particular user.

<div>

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption><p>Checking wins for self</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption><p>Checking wins for other users</p></figcaption></figure>

</div>

### a!glist

> This command shows all the active and ended giveaways in the particular server across all channels. This command also shows other information like giveaway host, giveaway winner of ended giveaways, and the channel the giveaway is in.&#x20;

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

This command sends a button to view all the giveaways in paginator (page embed) form, as shown below.&#x20;

<div>

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption><p>Page 1 (Ongoing Giveaway)</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption><p>Page 2 (Ongoing Giveaway)</p></figcaption></figure>

</div>

<div>

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption><p>Page 3 (Ended Giveaway)</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption><p>Page 4 (Ended Giveaway)</p></figcaption></figure>

</div>

### a!winrole (winroleset/remove)

> This command shows the roles that are to be added to the winner after they have won a giveaway. a!winrole set adds a new role to be added to the winners whereas a!winrole remove will delete the role to be added to winners.

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption><p>More than one role can be added too</p></figcaption></figure>

{% hint style="warning" %}
This command is a premium only command, to know more please goto the [premium](../premium.md) tab
{% endhint %}

### a!managerole

> This command allows you to assign a giveaway manager role. By using this command you dont need to give the giveaway host the `manage server` permission, as simply assigning this role to the host will allow them to host and control giveaways.

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
This command is a premium only command, to know more please goto the [premium](../premium.md) tab
{% endhint %}

## Giveaway Host Commands

### a!gstart

> This command is used to start giveaways in a particular channel. The format to use this command is `a!gstart <time> <winners> <prize>`. Once you have entered the parameters, Apollo will automatically delete your message and start a giveaway in that particular channel.\
> \
> For Example to host a giveaway with 2 winners, time of 1 hour and prize of Gold, we type in `a!gstart 1h 2 Gold`



<figure><img src="../.gitbook/assets/a!gstart.gif" alt=""><figcaption><p>Example giveaway</p></figcaption></figure>

### a!gend

> This command is used to end a particular giveaway in a particular channel. If there are more than one giveaways running at the same time then you can use `a!gend <messageid>` to end that particular giveaway, as we replace `<messageid>` with the id of the giveaway.

<figure><img src="../.gitbook/assets/a!gend.gif" alt=""><figcaption><p>Ending giveaway</p></figcaption></figure>

### a!greroll

This command rerolls the winner of a perticular giveaway. When multiple giveaways are running then you can use `a!greroll <messageid>` to reroll that particular giveaway. Here `<messageid>` is the id of the message of the giveaway.

<figure><img src="../.gitbook/assets/a!greroll.gif" alt=""><figcaption><p>Rerolling Giveaway</p></figcaption></figure>

## Giveaway Control Commands

### a!gwblacklist

> This command blacklists a particular user from reacting/participating in giveaways by automatically unreacting to giveaways in the particular server. This command only applies to the local server and not the global giveaway blacklist (i.e. the user can still participate in other giveaways hosted by apollo in other servers)\
> \
> Just type in `a!gwblacklist <@user>` to blacklist them from all giveaways in your server.

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption><p>User Successfully Blacklisted</p></figcaption></figure>

### a!gdelete

This command deletes the giveaway log from the a!glist database. To delete a particular giveaway just use the a!gdelete command followed by the giveaway message id that can be obtained either directly from the message or from the [a!glist](giveaways.md#a-glist) command.

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption><p>Bot confirming to delete the particular giveaway</p></figcaption></figure>

<div>

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption><p>Giveaway Successfully Deleted</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Original Giveaway Message also is deleted</p></figcaption></figure>

</div>
