---
layout: default
title: Collecting Metrics 2.5.1 & 2.5.2
permalink: priv-mgmt/collection-251-252
collection: priv-mgmt
---
---
### Privileged User Authentication

![calc logo](../img/calc.png){:style="width:40px;float:left;"}<br><br>
#### Where Do I Start? <br>
<p>
1. Start with the users identified in <a href="collection-26-25">Step 4 - Metric 2.5.</a> </p>
<p>
2. Exclude users that can log onto the network with <i>anything other than</i> a PIV or NIST approved credential. (Examples: One time password tokens, SMS PIN & Password, Username and Password).</p>

> •  Some users have multiple accounts - a user must be *excluded* if even one of their accounts lets them log onto the network with something other than a PIV or NIST approved credential.

> •  Users who have the *option* of PIV credential or Username/Password should also be excluded since PIV credential is not **_required._**

<p> 3. For the remaining users, include users that are technologically required through user based enforcement (UBE). This requires the user to use PIV credentials on all devices to access the network and disables the password. The users that have this enforcement should be counted.</p>
> •  See the [Searching Active Directory - PIV](../tools-tips/searchAD-PIV) page for information on querying for these users.
<p> 4. For the remaining users who have a PIV credential but who aren’t UBE or MBE, exclude users who can log onto the network without a PIV credential.</p>
<p> 5. Count the total number of unique users who have not been excluded in previous steps on this page and record number for Metric 2.5.1.</p>
<p> 6. Start with the users identified in Step 1 and exclude the users identified in Step 5.</p>
<p> 7. For each remaining account, does the account have the <b><i>ability</i></b> to log onto the network using a <i>username & password?</i> If it does, the user of the account should be counted.</p>
<p> 8. Count the total number of unique users found in Step 7 and record the number for Metric 2.5.2.</p>
