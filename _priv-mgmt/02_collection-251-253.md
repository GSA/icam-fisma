---
layout: default
title: Collecting Metrics 2.5.1, 2.5.2, 2.5.3
permalink: /priv-mgmt/collection-251-253
collection: priv-mgmt
---
---
### Privileged Network Users and Authentication ![calc logo](../img/calc.png){:style="width:40px;float:right;"}
### Where Do I Start?
<p>
1.	Identify the characteristics that make your agency’s network accounts privileged.</p>
>•	See <a href="../priv-mgmt/addl-info">Section Resources</a>  for examples of these characteristics. They are typically groups in Active Directory.
<p>
2. Search the user repository (Active Directory) for accounts with the values identified in Step 1.</p>
>•	See <a href="../tools-tips/searchAD"> [Tools & Tips for Active Directory](../tools-tips/searchAD) </a> or <a href="../tools-tips/searchAD-PIV ">Tools & Tips for Active Directory-PIV</a> for example searches.
<p>
3. Count the accounts in step 2 that are assigned to/ used by individual people (non-system).</p>
>•	See <a href="../tools-tips/searchAD">Tools & Tips for Active Directory</a> for an example of how to count objects using PowerShell.    
<p>     
4.	Identify the number of users of the accounts. Take care to eliminate duplicates from the count if two accounts are researched and identified to be assigned to the same person. Record this number for Metric 2.5.1.</p>
<p>
5.	Start with the users identified in Step 4 and exclude users that can log onto the network with <i>anything other</i> than through the machine-based or user-based enforcement of a two-factor PIV credential or other NIST 800-63 r3 Identity Assurance Level (IAL)3/Authenticator Assurance Level (AAL) 3/Federated Assurance Level (FAL) 3 credential. (Examples: One time password tokens, SMS PIN & Password, Username and Password). See <a href="../tools-tips/searchAD-PIV">Tools & Tips for Active Directory-PIV</a> for information on querying for these users. </p>

> a.	Some users have multiple accounts - a user must be *excluded* if even one of their accounts lets them log onto the network with something other than a PIV or NIST approved credential.

> b.	Users who have the *option* of a two-factor PIV credential or Username/Password should also be excluded since two-factor PIV credential is not <i><b>required</b></i>.
<p>
6.	Count the total number of unique users who have not been excluded in previous steps on this page and record number for Metric 2.5.2.</p>
<p>
7.	Take the users from Step 6 and <i>exclude</i> the users identified in Step 4.</p>
<p>
8.	For each remaining account, does the account have the ability to log onto the network using a username & password? If it does, the user of the account should be counted.</p>
<p>
9.	Count the total number of unique users found in Step 6 and record the number for the first part of Metric 2.5.3.
</p>
![aha logo](../img/aha.png){:style="width:45px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
John.smith.1 and john.smith.2 might both belong to the same person!
</div>
</div>

**Compensating Controls for Limited User Access**
<p>
1. If you <i>do</i> have users that use their username and password as their primary authentication method, identified in Step 6, please describe the policies, technologies, and controls in place that limit the users’ access when this login method is used. Record this information under the comments field of Metric 2.5.3.</p>
<p>
2. If you <i>don’t</i> have a policy, technology, and controls in place that limit users’ access when this login method is used, please respond with <i>No controls implemented</i>.</p>

•	For recommended compensating controls, please review the [Best Practices for Privileged User PIV Authentication Guidelines.](https://csrc.nist.gov/csrc/media/publications/white-paper/2016/04/21/best-practices-for-privileged-user-piv-authentication/final/documents/best-practices-privileged-user-piv-authentication.pdf)
