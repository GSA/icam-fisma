---
layout: default
title: Privileged Accounts and Users
collection: priv-mgmt
permalink: /priv-mgmt/

---
---
 <h3>This section covers FISMA metrics around privileged accounts and users (2.5.1, 2.5.2, 2.5.3, 2.5.4, 2.5.5, 2.5.6, 2.6.1, 2.6.2, 2.7.2, 2.8.2). </h3>
<img src="../img/graph.png" alt="logo"/>

### <b>Metrics 2.5.1-2.5.6 References:</b> [OMB M-18-02](https://insidecybersecurity.com/sites/insidecybersecurity.com/files/documents/oct2017/cs2017_OMB.pdf), [NIST 800-53r4 IA-2(2)](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf), [NIST SP 800-63](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-63-2.pdf)

### [Privileged Network Users and Authentication](collection-251-253)

| 2.5.1 | Number of privileged users with network accounts. (Exclude [non-user accounts](../tools-tips/fisma-def)) <b>(1)</b>  <img src="../img/recycle.png" alt="Chart logo" style="width:3%" align="middle">
| 2.5.2 | Number of privileged users (from 2.5.1.) that are required to authenticate to the network through the [machine-based or user-based enforcement](../tools-tips/searchad-piv) of a  two-factor PIV credential <b>(2)</b> or other NIST 800-63 r3 Identity Assurance Level (IAL)3/Authenticator Assurance Level (AAL) 3/Federated Assurance Level (FAL) 3 credential.
| 2.5.3 | Number of privileged users (from 2.5.1.) that use a username and password as their primary method for network authentication. Please describe compensating controls for limiting these users’ access in the comments field.

<b>(1)</b> An unprivileged network account is any account that is not a [privileged network account](../tools-tips/fisma-def).

<b>(2)</b>  For a person with one or more unprivileged network accounts, the person should be counted in the total only if a two-factor PIV Credential is necessary to authenticate to all network accounts. The enforcement of authentication may be accomplished via either user-based or machine-based configuration settings.

![recycle logo](../img/recycle.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
<p class="usa-alert-text"><H4>Save the result from Metric 2.5.1!</H4> You'll use the user information found here again for metrics 2.5.2, 2.5.3, 2.5.4 and 2.5.5.</p>  
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
    <p class="usa-alert-text"><H4>Why are Metrics 2.5.2 and 2.5.3 important?</H4>
    It is important to authenticate credentials when a user accesses a new network.
    Additionally, users must use a two-factor PIV credential to log onto the networks to mitigate attacks such as <i>Pass the Hash.</i> </p>

</div>
</div>

### [Privileged Users Covered by a Centralized Dynamic Access Management Solution](collection-254)

| 2.5.4 | Number of privileged users (from 2.5.1.) covered by a centralized dynamic access management solution that controls and monitors users’ access. ([NIST SP 800-53r4 AC-2(6)](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf))

![ribbon logo](../img/ribbon.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
    <p class="usa-alert-text"><H4>What is a centralized dynamic access management solution?</H4>
A centralized dynamic access management solution may be more commonly known as an Attribute Based Access Control (ABAC) model. These types of models provide an attribute-based approach to accommodate a wide breadth of access control policies and help simplify access control management.</p>
</div>
</div>

### [Privileged User Privilege Review](collection-255)

| 2.5.5 | Frequency with which privileged user privileges are reviewed, according to agency policy.

![ribbon logo](../img/ribbon.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
    <p class="usa-alert-text"><H4>Why is Metric 2.5.5 important?</H4></p>
A user needs the correct level of access to the right resources to fulfill their job function. Reviewing and correcting access supports least privilege, and policies such as segregation of duties.
</div>
</div>

### [Privileged User Network Accounts with Technical Controls](collection-256)

| 2.5.6 | Percent (%) of privileged users with network accounts that have a technical control limiting access to only trusted sites.

### Metrics 2.6.1-2.6.2 Reference: [NIST 800-53r4 IA-2(3)](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf)

### [Users with Privileged Local System Accounts and Users Required to Use Machine-based or User-based Enforcement of a Two-factor PIV or Other NIST Credential](collection-261-262)

| 2.6.1 | Number of users with [privileged local system accounts](../tools-tips/fisma-def) <b>(3)</b>. <img src="../img/recycle.png" alt="Chart logo" style="width:3%" align="middle">
| 2.6.2 | Number of users with [privileged local system accounts](../tools-tips/fisma-def) (from 2.6.1) are accessible through the Agency’s network in which the privileged user is required to authenticate to the network through the [machine-based or user-based enforcement](../tools-tips/fisma-def) of a two-factor [PIV](../tools-tips/fisma-def) credential or other NIST 800-63 r3 IAL3/AAL3/FAL3 credential.

<b>(3)</b> Do not report [privileged local system accounts](../tools-tips/fisma-def) that are not accessible on the network.

![recycle logo](../img/recycle.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
<p class="usa-alert-text"><H4>Save the result from Metric 2.6.1!</H4> You'll use the user information found here again for metric 2.6.2 and 2.8.2.</p>  
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
    <p class="usa-alert-text"><H4>Why are metrics 2.6.1 and 2.6.2 important?</H4></p>
    <ul>
      <li>  Understanding this user population helps to validate that they have the appropriate access across information systems.</li>
      <li> Issuing the appropriate credentials to user populations is meaningless unless agencies are requiring the use of these credentials.</li>
      </ul>
</div>
</div>

### [Network Accounts Assigned to Privileged Users](collection-272)

|2.7.2| Number of network accounts assigned to privileged users. (Exclude [non-user accounts](../tools-tips/fisma-def).)

### [Local System Accounts Assigned to Privileged Users](collection-282)

|2.8.2| Number of [local system accounts](../tools-tips/fisma-def) assigned to privileged users.
