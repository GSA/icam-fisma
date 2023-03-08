---
layout: default
title: Introduction
permalink: /
---
---
There are <b>13</b> ICAM-related metrics in the <a href="https://www.dhs.gov/sites/default/files/publications/FY%202018%20CIO%20FISMA%20Metrics_V2_Final.pdf"> FY18 CIO FISMA Metrics</a>, including several new metrics that have not been collected in previous years. FY18 ICAM-related metrics can be found under Section 2 (Protect) of the guidance and below.

<html>
<head>
<style>
#metrics {
    border-collapse: collapse;
    width: 100%;
}

#metrics td, #metrics th {
    border: 1px solid black;
    padding: 8px;
}

#metrics th {
    padding-top: 15px;
    padding-bottom: 15px;
    padding-left: 15px;
    padding-right: 15px;
    text-align: center;
    background-color: #e1f3f8;
}
</style>
</head>
<body>

<table id="metrics">
  <tr>
    <th><b>METRIC</b></th>
    <th><b>DESCRIPTION</b></th>

  </tr>
  <tr>
    <td><a href="unpriv-mgmt/collection-241"><b>2.4.1</b></a></td>
    <td>Number of unprivileged users with network accounts.<sup>1</sup> (Exclude <a href="tools-tips/fisma-def"> non-user accounts)</a></td>
    </tr>
    <tr>
      <td><a href="unpriv-mgmt/collection-242"><b>2.4.2</b></a></td>
      <td>Number of unprivileged users (from 2.4.1) that are required to authenticate to the network through the <a href="tools-tips/searchad-piv"> machine-based</a> or <a href="tools-tips/searchad-piv"> user-based enforcement</a> of a two-factor PIV credential<sup>2</sup> or other NIST 800-63 r3 Identity Assurance Level (IAL)3/Authenticator Assurance Level (AAL) 3/Federated Assurance Level (FAL) 3 credential.<sup>3</sup></td>
  </tr>
  <tr>
  <td><a href="unpriv-mgmt/collection-243"><b>2.4.3</b></a></td>
    <td>Number of unprivileged users (from 2.4.1) that use a username and password as their primary method for network authentication. Please describe compensating controls for limiting these users’ access in the comments field.</td>
  </tr>
  <tr>
  <td><a href="unpriv-mgmt/collection-244"><b>2.4.4</b></a></td>
    <td>Number of unprivileged users (from 2.4.1) covered by a centralized dynamic access management solution that controls and monitors users’ access. <a href="http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf"> (NIST SP 800-53r4 AC-2(6))</a>)</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/collection-251"><b>2.5.1</b></a></td>
    <td>Number of privileged users with network accounts.<sup>1</sup> (Exclude <a href="tools-tips/fisma-def"> non-user accounts</a>)</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/collection-252"><b>2.5.2</b></a></td>
    <td>Number of privileged users (from 2.5.1) that are required to authenticate to the network through the <a href="tools-tips/searchad-piv"> machine-based</a> or <a href="tools-tips/searchad-piv"> user-based enforcement</a> of a two-factor PIV credential<sup>2</sup> or other NIST 800-63 r3 Identity Assurance Level (IAL)3/Authenticator Assurance Level (AAL) 3/Federated Assurance Level (FAL) 3 credential.<sup>3</sup></td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/collection-253"><b>2.5.3</b></a></td>
    <td>Number of privileged users (from 2.5.1) that use a username and password as their primary method for network authentication. Please describe compensating controls for limiting these users’ access in the comments field.</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/collection-254"><b>2.5.4</b></a></td>
    <td>Number of privileged users (from 2.5.1) covered by a centralized dynamic access management solution that controls and monitors users’ access. <a href="http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf"> (NIST SP 800-53r4 AC-2(6))</a>)</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/collection-255"><b>2.5.5</b></a></td>
    <td>Frequency with which privileged user privileges are reviewed, according to agency policy.</td>
  </tr>
  <tr>
    <td><a href="network-local/collection-261"><b>2.6.1</b></a></td>
    <td>Number of users with <a href="tools-tips/fisma-def"> privileged local system accounts.</a><sup>4</sup></td>
  </tr>
  <tr>
    <td><a href="network-local/collection-262"><b>2.6.2</b></a></td>
    <td>Number of users with <a href="tools-tips/fisma-def"> privileged local system accounts </a> (from 2.6.1) are accessible through the Agency’s network in which the privileged user is required to authenticate to the network through the <a href="tools-tips/searchad-piv"> machine-based</a> or <a href="tools-tips/searchad-piv"> user-based enforcement</a> of a two-factor <a href="tools-tips/fisma-def"> PIV </a> credential or other NIST 800-63 r3 IAL3/AAL3/FAL3 credential.</td>
  </tr>
  <tr>
    <td><a href="network-local/collection-27"><b>2.7</b></a></td>
    <td>Number of High Value Asset (HVA) systems<sup>5</sup> that require all government and contractor users (100% privileged and unprivileged) to authenticate through the <a href="tools-tips/searchad-piv"> machine-based</a> or <a href="tools-tips/searchad-piv"> user-based enforcement</a> of a two-factor <a href="tools-tips/fisma-def">PIV</a> credential or other NIST 800-63 r3 IAL3/AAL3 credential.</td>
  </tr>
  <tr>
    <td><a href="network-local/collection-271"><b>2.7.1</b></a></td>
    <td>Number of HVA systems assessed by DHS, a third-party, or independent entity (per M-17-09) that determined machine-based or user-based enforcement of a two-factor PIV credential (as described in 2.7.) is not required due to mitigating security capabilities.</td>
  </tr>
</table>
</body>
</html>

Data collected from these metrics can help your agency prioritize and guide decisions around resource allocation to assure ICAM Program effectiveness. The ultimate goal of these metrics is to enable your agency to ensure the right people have the right access to the right data at the right time. ICAM program advancement is an incremental process and unique to each agency’s mission and business needs.

The GSA FICAM Program has worked with DHS, OMB, and others to develop practical guidance to help your agency collect the data for the ICAM-related FISMA metrics. This guidance is intended to help you logically navigate and interpret the metrics to decrease your reporting time and increase usability and understanding. We hope that senior leadership will have a better “apples-to-apples” comparison across agencies if all agencies have a clearer understanding of what the metrics represent and how to collect and report them.  

---
<sup> 1 </sup> An unprivileged network account is any account that is not a <a href="tools-tips/fisma-def"> privileged network account</a>.

<sup> 2 </sup> For a person with one or more unprivileged network accounts, the person should be counted in the total only if a two-factor PIV Credential is necessary to authenticate to all network accounts. The enforcement of authentication may be accomplished via either user-based or machine-based configuration settings.

<sup> 3 </sup> For additional information, refer to <a href="https://pages.nist.gov/800-63-3/"> NIST SP 800-63.</a>

<sup> 4 </sup> Do not report <a href="tools-tips/fisma-def"> privileged local system accounts </a> that are not accessible on the network.

<sup> 5 </sup> HVA as defined in <a href="https://www.whitehouse.gov/sites/whitehouse.gov/files/omb/memoranda/2017/m-17-09.pdf"> M-17-09. </a> OMB will leverage existing data sources for the denominator of HVA related metrics.
