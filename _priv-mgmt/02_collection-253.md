---
layout: default
title: Collecting Metric 2.5.3
permalink: /priv-mgmt/collection-253
collection: priv-mgmt
---
---
### Privileged Network Users and Authentication ![calc logo](../img/calc.png){:style="width:40px;float:right;"}
#### Where Do I Start?
##### Part 1:
1.	Take the users identified in [Metric 2.5.2](../priv-mgmt/collection-252) and <i>exclude</i> the users from [Metric 2.5.1](../priv-mgmt/collection-251).
2.	For each remaining account, does the account have the ability to log onto the network using a username & password? If it does, the user of the account should be counted.
3.	Count the total number of users identified in step 2 and record the number for the first part of <b>Metric 2.5.3.</b>

##### Part 2:
4.  If you <i>do</i> have users that use their username and password as their primary authentication method, identified in Step 2 above, please describe the policies, technologies, and controls in place that limit the users’ access when this login method is used. Record this information under the comments field of <b>Metric 2.5.3</b>.
5.  If you <i>don’t</i> have a policy, technology, and controls in place that limit users’ access when this login method is used, please respond with <i>No controls implemented</i>.

![ribbon logo](../img/ribbon.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
    <p class="usa-alert-text"><H4>Why is Metric 2.5.3 important?</H4>
    It is important to authenticate credentials when a user accesses a new network.
    Additionally, users must use a two-factor PIV credential to log onto the networks to mitigate attacks such as <i>Pass the Hash.</i> </p>

</div>
</div>

![focus logo](../img/focus.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text"><H4>Additional Information</H4>
For recommended compensating controls, please review the <a href="https://csrc.nist.gov/csrc/media/publications/white-paper/2016/04/21/best-practices-for-privileged-user-piv-authentication/final/documents/best-practices-privileged-user-piv-authentication.pdf"> Best Practices for Privileged User PIV Authentication Guidelines.</a>

</div>
</div>
