---
layout: default
title: Unprivileged Network Users
permalink: /unpriv-mgmt/
collection: unpriv-mgmt
---
---
<h3>This section covers FISMA metrics around unprivileged networks and users (2.4.1, 2.4.2, 2.4.3, 2.4.4, 2.7.1, 2.8.1).</h3>
<img src="../img/graph.png" alt="logo"/>

### <b>Metrics 2.4.1-2.4.4 References:</b> [OMB M-18-02](https://insidecybersecurity.com/sites/insidecybersecurity.com/files/documents/oct2017/cs2017_OMB.pdf), [NIST 800-53r4 IA-2(2)](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf), [NIST SP 800-63](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-63-2.pdf)

### [Unprivileged Network Users and Authentication](collection-241-243)

| 2.4.1 | Number of unprivileged users with network accounts.(Exclude [non-user accounts](../tools-tips/fisma-def)) <b>(1)</b> <img src="../img/recycle.png" alt="Chart logo" style="width:3%" align="middle">
| 2.4.2 | Number of unprivileged users (from 2.4.1) that are required to authenticate to the network through the [machine-based or user-based enforcement](../tools-tips/searchad-piv) of a two-factor PIV credential <b>(2)</b> or other NIST 800-63 r3 Identity Assurance Level (IAL)3/Authenticator Assurance Level (AAL) 3/Federated Assurance Level (FAL) 3 credential.
| 2.4.3 | Number of unprivileged users (from 2.4.1) that use a username and password as their primary method for network authentication. Please describe compensating controls for limiting these users’ access in the comments field.

<b>(1)</b> An unprivileged network account is any account that is not a [privileged network account](../tools-tips/fisma-def).

<b>(2)</b> For a person with one or more unprivileged network accounts, the person should be counted in the total only if a two-factor PIV Credential is necessary to authenticate to all network accounts. The enforcement of authentication may be accomplished via either user-based or machine-based configuration settings.

![recycle logo](../img/recycle.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
<p class="usa-alert-text"><H4>Save the result from Metric 2.4.1!</H4> You'll use the user information found here again for metrics 2.4.2, 2.4.3, and 2.4.4.</p>  
</div>
</div>
![ribbon logo](../img/ribbon.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
    <p class="usa-alert-text"><H4>Why are Metrics 2.4.2 & 2.4.3 important?</H4>
    It is important to authenticate credentials when a user accesses a new network.
    Additionally, users must use a two-factor PIV credential to log onto the networks to mitigate attacks such as <i>Pass the Hash.</i> </p>

</div>
</div>

### [Unprivileged Users Covered by a Centralized Dynamic Access Management Solution](collection-244)

| 2.4.4 | Number of users (from 2.4.1.) covered by a centralized dynamic access management solution that controls and monitors users’ access. ([NIST SP 800-53r4 AC-2(6)](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf))

![ribbon logo](../img/ribbon.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
    <p class="usa-alert-text"><H4>Why is Metric 2.4.4 important?</H4>
A centralized dynamic access management solution model is similar to an Attribute Based Access Control (ABAC) model. These types of models provide an attribute-based approach to accommodate a wide breadth of access control policies and help simplify access control management.</p>
</div>
</div>

### [Network Accounts Assigned to Unprivileged Users](collection-271)

| 2.7.1 | Number of network accounts assigned to unprivileged users. (Exclude [non-user accounts](../tools-tips/fisma-def)).

### [Local System Accounts Assigned to Unprivileged Users](collection-281)

| 2.8.1 | Number of [local system accounts](../tools-tips/fisma-def) assigned to unprivileged users.
