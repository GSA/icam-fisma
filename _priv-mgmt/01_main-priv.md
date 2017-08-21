---
layout: default
title: Privileged Accounts and Users
permalink: priv-mgmt/main-priv
collection: priv-mgmt
---
### This section covers FISMA metrics around privileged accounts and users (2.6, 2.6.1, 2.5, 2.5.1, 2.5.2, 2.7, 2.8).
![Chart logo](../img/graph.png){:style="width:8%;"}{:style="float:left"}
<br> <br> <br>
### [Privileged Network Accounts & Users](collection-26-25)

| 2.6 | Number of privileged network accounts assigned to users. (Exclude unprivileged network accounts and non-user accounts.)
| 2.6.1 | Number of privileged shared network accounts. (Exclude unprivileged network accounts and non-user accounts.)
| 2.5 | Number of users with privileged network accounts. (Exclude unprivileged network accounts and non-user accounts.)

### [Privileged User Authentication](collection-251-252)

| 2.5.1 | Number of users (from 2.5) technologically required to log onto the network with a two-factor PIV credential or other NIST credential.
| 2.5.2| Number of users (from 2.5) allowed to use username and password as their primary method for network authentication.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why are Metrics 2.5.1 & 2.5.2 important?</H4>
    It is important to authenticate credentials when a user accesses a new network. Additionally, users must use a PIV credential to log onto the networks to mitigate attacks such as Pass the Hash </p>
</div>
</div>

### [Users with Privileged Local System Accounts and Users Required to Use PIV credentials](collection-27-28)

|2.7| Number of users with privileged local system accounts.
|2.8| Number of users with privileged local system accounts (from 2.7) technologically required to log onto the system with a two-factor PIV credential or other NIST credential.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why are metrics 2.7 and 2.8 important?</H4>
    <p>• Understanding this user population helps to validate that they have the appropriate access across information systems</p>
    <p>• Issuing the appropriate credentials to user populations is meaningless unless agencies are requiring the use of these credentials</p>
    </p>
</div>
</div>
<br>
