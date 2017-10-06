---
layout: default
title: Collecting Metrics 2.4.1 and 2.4.2
permalink: unpriv-mgmt/collection-241-242
collection: unpriv-mgmt
---
---
### Unprivileged User Authentication ![calc logo](../img/calc.png){:style="width:40px;float:right;"}
### Where Do I Start?
<p>
1. Start with the users identified in <a href="collection-26-24">Step 4 - Metric 2.4.</a> </p>
<p>
2. Exclude users that can log onto the network with <i>anything other than</i> a PIV or NIST approved credential. (Examples: One time password tokens, SMS PIN & Password, Username and Password).</p>
<ul>
<li>Some users have multiple accounts - a user must be <i>excluded</i> if even one of their accounts lets them log onto the network with something other than a PIV or NIST approved credential.</li>
<li>Users who have the <i>option</i> of PIV credential or Username/Password should also be excluded since PIV credential is not <b><i>required.</i></b></li>
</ul>
<p> 3. For the remaining users, include users that are technologically required through user based enforcement (UBE). This requires the user to use PIV credentials on all devices to access the network and disables the password. The users that have this enforcement should be counted.</p>
<ul>
<li>See <a href="../tools-tips/searchAD-PIV">Searching Active Directory - PIV</a> for information on querying for these users.</li>
</ul>
<p> 4. For the remaining users who have a PIV credential but who aren’t UBE or MBE, exclude users who can log onto the network without a PIV credential.</p>
<p> 5. Count the total number of unique users who have not been excluded in previous steps on this page and record number for Metric 2.4.1.</p>
<p> 6. Start with the users identified in Step 1 and exclude the users identified in Step 5.</p>
<p> 7. For each remaining account, does the account have the <b><i>ability</i></b> to log onto the network using a <i>username & password?</i> If it does, the user of the account should be counted.</p>
<p> 8. Count the total number of unique users found in Step 7 and record the number for Metric 2.4.2.</p>

![pencil logo](../img/pencil.png){:style="width:45px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
    <p class="usa-alert-text"><H4>Step 3 Example</H4>
    Bob normally uses his PIV credential to log onto the network. That PIV credential is associated with his AD account bob123. However, Bob sometimes uses a VPN from home. When he logs into the network through the VPN, he uses his username and password and a one time password. Bob would be excluded from this count because he is not required to log onto the network with his PIV credential.</p>
</div>
</div>
