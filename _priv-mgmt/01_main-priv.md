---
layout: default
title: Privileged Accounts and Users
permalink: priv-mgmt/main-priv
collection: priv-mgmt
---
This section covers FISMA metrics around privileged accounts and users (2.7, 2.7.1, 2.7.2, 2.5, 2.5.1, 2.5.2, 2.8, 2.9, 2.10, 2.11 and 2.12) 

>![Chart logo](../img/graph.png){:style="width:8%;"}

### [Privileged Network Accounts & Users](collection-25-27)

| 2.7. | Number of privileged network accounts assigned to users. (Exclude unprivileged network accounts and non-user accounts.)
| 2.7.1 | Number of privileged shared network accounts. (Exclude unprivileged network accounts and non-user accounts.)
| 2.7.2 | Number of individual users assigned to privileged shared network accounts (from 2.7.1.)
| 2.5. | Number of users with privileged network accounts. (Exclude unprivileged network accounts and non-user accounts.) ![Chart logo](../img/recycle.png){:style="width:3%;"}

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why is Metric 2.7.2 important?</H4>
    Shared accounts generally have less accountability associated than non-shared accounts. Privileged shared accounts run a higher risk to an organization since their compromise might not be noticed as quickly.</p> 
</div>
</div>

### [Privileged User Authentication](collection-251-252)

| 2.5.1 | Number of users (from 2.5) technologically required to log onto the network with a two-factor PIV card or other NIST Level of Assurance (LOA) 4 credential.
| 2.5.2| Number of users (from 2.5) allowed to use username and password as their primary method for network authentication.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why are Metrics 2.5.1 and 2.5.2 important?</H4>
    It is important to authenticate credentials when a user accesses a new network. Additionally, users must use PIV to log onto the networks to mitigate attacks such as Pass the Hash.</p> 
</div>
</div>

### [Non-User Privileged Network Accounts](collection-28)

|2.8| Number of non-user privileged network accounts. (Exclude unprivileged network accounts and privileged network accounts assigned to a user.)

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why is Metric 2.8 important?</H4>
    Privileged accounts provide greater access rights than non-privileged accounts. Some of these accounts could be thought of as having the "keys to the kingdom". Although an account may be considered non-user, it may not stop someone from using it to log onto a network if compromised. Since they're not associated with a user, it is more difficult to identify accountability for the account's actions.

It is important to understand the makeup of all types of privileged accounts so you can take steps to avoid the risk of compromise.</p> 
</div>
</div>


