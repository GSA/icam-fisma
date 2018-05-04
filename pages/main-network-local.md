---
layout: default
title: Network and Local System Accounts
collection: network-local
permalink: /network-local/

---
---
### This section covers FISMA metrics around Network and Local System Accounts (2.6.1-2.6.2).
<img src="../img/graph.png" alt="logo"/>

![focus logo](../img/focus.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text"><H4>Please refer to the following guidance for Metrics 2.6.1-2.6.2:</H4>
<p>
 <a href="http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf"> NIST 800-53r4 IA-2(3)</a>
</p>
</div>
</div>

| [2.6.1](../network-local/collection-261) | Number of users with [privileged local system accounts.](../tools-tips/fisma-def) <sup>4</sup> <img src="../img/recycle.png" alt="Chart logo" style="width:3%" align="middle">
| [2.6.2](../network-local/collection-262) | Number of users with [privileged local system accounts](../tools-tips/fisma-def) (from 2.6.1) are accessible through the Agency’s network in which the privileged user is required to authenticate to the network through the [machine-based enforcement](../tools-tips/searchad-piv) or [user-based enforcement](../tools-tips/searchad-piv) of a two-factor [PIV](../tools-tips/fisma-def) credential or other NIST 800-63 r3 IAL3/AAL3/FAL3 credential.

![focus logo](../img/focus.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text"><H4>Please refer to the following guidance for Metrics 2.7-2.7.1:</H4>
<p>
<a href="https://insidecybersecurity.com/sites/insidecybersecurity.com/files/documents/oct2017/cs2017_OMB.pdf"> OMB M-18-02, </a>
<a href="https://pages.nist.gov/800-63-3/"> NIST SP 800-63 </a>
</p>
</div>
</div>

| [2.7](../network-local/collection-27) | Number of High Value Asset (HVA) systems<sup>5</sup> that require all government and contractor users (100% privileged and unprivileged) to authenticate through the [machine-based](../tools-tips/searchad-piv) or [user-based enforcement](../tools-tips/searchad-piv)of a two-factor [PIV](../tools-tips/fisma-def) credential or other NIST 800-63 r3 IAL3/AAL3 credential.<img src="../img/recycle.png" alt="Chart logo" style="width:3%" align="middle">
| [2.7.1](../network-local/collection-271) | Number of HVA systems assessed by DHS, a third-party, or independent entity (per <a href="https://www.whitehouse.gov/sites/whitehouse.gov/files/omb/memoranda/2017/m-17-09.pdf"> M-17-09</a>). that determined machine-based or user-based enforcement of a two-factor PIV credential (as described in 2.7). is not required due to mitigating security capabilities.

---
<sup>4</sup> Do not report [privileged local system accounts](../tools-tips/fisma-def) that are not accessible on the network.

<sup>5</sup> HVA as defined in <a href="https://www.whitehouse.gov/sites/whitehouse.gov/files/omb/memoranda/2017/m-17-09.pdf"> M-17-09.</a> OMB will leverage existing data sources for the denominator of HVA related metrics.
