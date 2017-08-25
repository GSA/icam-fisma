---
layout: default
title: Collecting Metrics 2.4.1 and 2.4.2
permalink: unpriv-mgmt/collection-241-242
collection: unpriv-mgmt
---
---
### Unprivileged User Authentication

![calc logo](../img/calc.png){:style="width:40px;float:left;"}<br><br>
#### Where Do I Start? <br>
<p>
1. Start with the users identified in <a href="collection-26-24">Step 4 - Metric 2.4.</a> </p>
<p>
2. Exclude users that can log onto the network with <i>anything other than</i> a PIV or NIST approved credential. (Examples: One time password tokens, SMS PIN & Password, Username and Password).</p>

> •  Some users have multiple accounts - a user must be *excluded* if even one of their accounts lets them log onto the network with something other than a PIV or NIST approved credential.

> •  Users who have the *option* of PIV credential or Username/Password should also be excluded since PIV credential is not **_required._**

<p> 3. For the remaining users, include users that are technologically required through user based enforcement (UBE). This requires the user to use PIV credentials on all devices to access the network and disables the password. The users that have this enforcement should be counted.</p>
> •  See the [Searching Active Directory - PIV](../tools-tips/searchAD-PIV) page for information on querying for these users.
<p> 4. For the remaining users who have a PIV credential but who aren’t UBE or MBE, exclude users who can log onto the network without a PIV credential.</p>
<p> 5. Count the total number of unique users who have not been excluded in previous steps on this page and record number for Metric 2.4.1.</p>
<p> 6. Start with the users identified in Step 1 and exclude the users identified in Step 5.</p>
<p> 7. For each remaining account, does the account have the <b><i>ability</i></b> to log onto the network using a <i>username & password?</i> If it does, the user of the account should be counted.</p>
<p> 8. Count the total number of unique users found in Step 7 and record the number for Metric 2.4.2.</p>

![ribbon logo](../img/ribbon.png){:style="width:40px;float:left;"}
<div class="usa-alert usa-alert;">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why are Metrics 2.4.1 & 2.4.2 important?</H4>
    It is important to authenticate credentials when a user accesses a new network. Additionally, users must use a PIV credential to log onto the networks to mitigate attacks such as <i>Pass the Hash</i> </p>
</div>
</div>

![pencil logo](../img/pencil.png){:style="width:45px;float:left;"}
<div class="usa-alert usa-alert;">
<div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Step 3 Example</H4>
    Bob normally uses his PIV credential to log onto the network. That PIV credential is associated with his AD account bob123. However, Bob sometimes uses a VPN from home. When he logs into the network through the VPN, he uses his username and password and a one time password. Bob would be excluded from this count because he is not required to log onto the network with his PIV credential.</p>
</div>
</div>
