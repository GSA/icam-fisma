---
layout: default
title: Collecting Metric 2.5.2
permalink: /priv-mgmt/collection-252
collection: priv-mgmt
---
---
### Privileged Network Users and Authentication ![calc logo](../img/calc.png){:style="width:40px;float:right;"}
#### Where Do I Start?

1.	Start with the users identified in [Metric 2.5.1](../priv-mgmt/collection-251) and exclude users that can log onto the network with <i>anything other</i> than through the machine-based or user-based enforcement of a two-factor PIV credential or other NIST 800-63 r3 Identity Assurance Level (IAL)3/Authenticator Assurance Level (AAL) 3/Federated Assurance Level (FAL) 3 credential. (i.e., one time password tokens, sms pin & password, username and password). Please see <a href="../tools-tips/searchAD-PIV">Tools & Tips for Active Directory-PIV</a> for information on querying for these users.
> a.	Some users have multiple accounts - a user must be *excluded* if even one of their accounts lets them log onto the network with something other than a PIV or NIST approved credential.
> b.	Users who have the *option* of a two-factor PIV credential or Username/Password should also be excluded since two-factor PIV credential is not <i><b>required</b></i>.

2.	Count the total number of unique users who have not been excluded in previous steps on this page and record number for <b>Metric 2.5.2</b>.

![ribbon logo](../img/ribbon.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
    <p class="usa-alert-text"><H4>Why is Metric 2.5.2 important?</H4>
    It is important to authenticate credentials when a user accesses a new network.
    Additionally, users must use a two-factor PIV credential to log onto the networks to mitigate attacks such as <i>Pass the Hash.</i> </p>

</div>
</div>
