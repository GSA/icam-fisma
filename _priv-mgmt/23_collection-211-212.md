---
layout: default
title: Collecting Metrics 2.11 & 2.12
permalink: priv-mgmt/collection-211-212
collection: priv-mgmt
---
## Users with Privileged Local System Accounts and Users Required to Use PIV/LOA 4
>![Calculator logo](../img/calc.png){:style="width:5%;"}

1. Identify the user population with privileged local system accounts.
> •  These users will typically support the administration of systems that run and make up the infrastructure.\\
•  These users may have groupsor some other access rights associated with the account that gives them privileged access to the local system.\\
•  The accounts may be built-in administrative accounts such as root on Unix-like systems.\\
•  Some local system accounts may have elevated privileges through built-in utilities such as SUDO. These accounts should be identified as well.
2. Count the number of individual users (people) with these accounts. A user with 5 privileged accounts counts once. Record this number for Metric 2.11.
3. For each of the users’ accounts identified in Metric 2.11, determine if the local system that allows a user to authenticate to the account requires authentication with a PIV or other LOA4 credential.
4. If yes, for all of the user’s privileged local accounts, count this user. If no for 1 or more of a user’s accounts, do not count the user. Record this number for Metric 2.12.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Don't Forget:</H4>
    •  Network Administrators 
    <br>•  Database Administrators
    <br>•  UNIX System Administrators
    <br>•  Mainframe Administrators
    <br>•  Web Server Administrators
    <br>•  Email Server Administrators
    </p>
</div>
</div>
