---
layout: default
title: Collecting Metrics 2.7 & 2.8
permalink: priv-mgmt/collection-27-28
collection: priv-mgmt
---
---
### Users with Privileged Local System Accounts and Users Required to Use PIV/NIST Approved Credentials

![calc logo](../img/calc.png){:style="width:40px;float:left;"}<br><br>
#### Where Do I Start? <br>
<p>
1. Identify the user population with privileged local system accounts.</p>
> •  These users will typically support the administration of systems that run and make up the infrastructure.

> •  These users may have *groups* or some other *access rights* associated with the account that gives them privileged access to the local system.

> •  The accounts may be built-in administrative accounts such as root on Unix-like systems.

> •  Some local system accounts may have elevated privileges through built-in utilities such as SUDO. These accounts should be identified as well.

<p> 2. Count the number of individual users (people) with these accounts. A user with 5 privileged accounts counts once. Record this number for Metric 2.7.</p>
<p> 3. For each of the users’ accounts identified in Metric 2.7, determine if the local system that allows a user to authenticate to the account requires authentication with a PIV or other NIST approved credential.</p>
<p> 4. If yes, for all of the user’s privileged local accounts, count this user. If no for 1 or more of a user’s accounts, do not count the user. Record this number for Metric 2.8.</p>

![light bulb logo](../img/ahabrn.png){:style="width:45px;float:left;"}
<div class="usa-alert usa-alert;">
  <div class="usa-alert-body">
  <p class="usa-alert-text"><H4>Don't Forget:</H4>
•  Network Administrators
<br>•  Database Administrators
<br>•  UNIX System Administrators
<br>•  Mainframe Administrators
<br>•  Web Server Administrators
<br>•  Email Server Administrators</p>
</div>
</div>
