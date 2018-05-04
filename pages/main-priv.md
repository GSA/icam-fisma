---
layout: default
title: Privileged Network Users
collection: priv-mgmt
permalink: /priv-mgmt/
---
---
### This section covers FISMA metrics around privileged network users (2.5.1-2.5.5).
<img src="../img/graph.png" alt="logo"/>

![focus logo](../img/focus.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text"><H4>Please refer to the following guidance for Metrics 2.5.1-2.5.5:</H4>
<p>
 <a href="https://insidecybersecurity.com/sites/insidecybersecurity.com/files/documents/oct2017/cs2017_OMB.pdf"> OMB M-18-02, </a>
 <a href="http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf"> NIST 800-53r4 IA-2(1), </a>
 <a href="https://pages.nist.gov/800-63-3/"> NIST SP 800-63 </a>
</p>
</div>
</div>

| [2.5.1](../priv-mgmt/collection-251) | Number of privileged users with network accounts.<sup>1</sup>  (Exclude [non-user accounts](../tools-tips/fisma-def))<img src="../img/recycle.png" alt="Chart logo" style="width:3%" align="middle">
| [2.5.2](../priv-mgmt/collection-252) | Number of privileged users (from 2.5.1.) that are required to authenticate to the network through the [machine-based](../tools-tips/searchad-piv) or [user-based enforcement](../tools-tips/searchad-piv) of a two-factor PIV credential<sup>2</sup> or other NIST 800-63 r3 Identity Assurance Level (IAL)3/Authenticator Assurance Level (AAL) 3/Federated Assurance Level (FAL) 3 credential.<sup>3</sup>
| [2.5.3](../priv-mgmt/collection-253) | Number of privileged users (from 2.5.1.) that use a username and password as their primary method for network authentication. Please describe compensating controls for limiting these users’ access in the comments field.
| [2.5.4](../priv-mgmt/collection-254) | Number of privileged users (from 2.5.1.) covered by a centralized dynamic access management solution that controls and monitors users’ access. ([NIST SP 800-53r4 AC-2(6)](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf))
| [2.5.5](../priv-mgmt/collection-255) | Frequency with which privileged user privileges are reviewed, according to agency policy.


---
<sup> 1 </sup> An unprivileged network account is any account that is not a [privileged network account](../tools-tips/fisma-def).

<sup> 2 </sup> For a person with one or more unprivileged network accounts, the person should be counted in the total only if a two-factor PIV Credential is necessary to authenticate to all network accounts. The enforcement of authentication may be accomplished via either user-based or machine-based configuration settings.

<sup> 3 </sup> For additional information, refer to <a href="https://pages.nist.gov/800-63-3/"> NIST SP 800-63.</a>
