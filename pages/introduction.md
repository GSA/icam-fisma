---
layout: default
title: Introduction
permalink: /
---
---
There are <b>21</b> ICAM-related metrics in the <a href="https://www.dhs.gov/sites/default/files/publications/FY%202018%20CIO%20FISMA%20Metrics_V1_Final%20508.pdf"> FY18 CIO FISMA Metrics</a>, including several new metrics that have not been collected in previous years. FY18 ICAM-related metrics can be found under Section 2 (Protect) of the guidance and below.

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
    <td><a href="id-access/"><b>2.3. NEW</b></a></td>
    <td>Date of issuance of an <a href="tools-tips/fisma-def">enterprise-level</a> Identity, Credential, and Access Management policy. <a href="https://www.whitehouse.gov/omb/circulars_a130_a130trans4">(OMB Circular A-130</a>, <a href="https://www.dhs.gov/homeland-security-presidential-directive-12"> Homeland Security Presidential Directive 12 (HSPD-12)</a>, <a href="http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf"> NIST SP 800-53r4 AC-6(7))</a></td>

  </tr>
  <tr>
    <td><a href="id-access/"><b>2.3.1 NEW</b></a></td>
    <td><a href="tools-tips/fisma-def">Enterprise-level</a> Identity, Credential, and Access Management policy contains processes for the review of user privileges, provisioning privileges upon entry, revoking privileges upon exit, and modifying privileges based on changes in duties. (e.g. role based access control).</td>
  </tr>
  <tr>
    <td><a href="unpriv-mgmt/"><b>2.4.1</b></a></td>
    <td>Number of unprivileged users with network accounts. (Exclude <a href="tools-tips/fisma-def"> non-user accounts</a>)</td>
  </tr>
  <tr>
    <td><a href="unpriv-mgmt/"><b>2.4.2</b></a></td>
    <td>Number of uprivileged users (from 2.4.1 that are required to authenticate to the network through the <a href="tools-tips/searchad-piv"> machine-based or user-based enforcement</a> of a two-factor PIV credential or other <a href="http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-63-3.pdf"> NIST 800-63 r3</a> Identity Assurance Level (IAL)3/Authenticator Assurance Level (AAL) 3/Federated Assurance Level (FAL) 3 credential. </td>
  </tr>
  <tr>
    <td><a href="unpriv-mgmt/"><b>2.4.3</b></a></td>
    <td>Number of unprivileged users (from 2.4.1) that use a username and password as their primary method for network authentication. Please describe compensating controls for limiting these users’ access in the comments field.</td>
  </tr>
  <tr>
    <td> <a href="unpriv-mgmt/"><b>2.4.4 NEW</b></a></td>
    <td> Number of unprivileged users (from 2.4.1) covered by a centralized dynamic access management solution that controls and monitors users’ access. (<a href="http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf"> NIST SP 800-53r4 AC-2(6)</a>)</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/"><b>2.5.1</b></a></td>
    <td>Number of privileged users with network accounts. (Exclude <a href="tools-tips/fisma-def"> non-user accounts</a>)</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/"><b>2.5.2</b></a></td>
    <td>Number of privileged users (from 2.5.1 that are required to authenticate to the network through the <a href="tools-tips/searchad-piv"> machine-based or user-based enforcement</a> of a two-factor PIV credential or other <a href="http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-63-3.pdf"> NIST 800-63 r3</a> Identity Assurance Level (IAL)3/Authenticator Assurance Level (AAL) 3/Federated Assurance Level (FAL) 3 credential. </td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/"><b>2.5.3</b></a></td>
    <td>Number of privileged users (from 2.5.1) that use a username and password as their primary method for network authentication. Please describe compensating controls for limiting these users’ access in the comments field.</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/"><b>2.5.4 NEW</b></a></td>
    <td> Number of privileged users (from 2.5.1) covered by a centralized dynamic access management solution that controls and monitors users’ access. (<a href="http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf"> NIST SP 800-53r4 AC-2(6)</a>)</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/"><b>2.5.5 NEW</b></a></td>
    <td>Frequency with which privileged user privileges are reviewed, according to agency policy.</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/"><b>2.6.1</b></a></td>
    <td>Number of users with <a href="tools-tips/fisma-def">privileged local system accounts.</a></td>
  </tr>
  <tr>
    <td> <a href="priv-mgmt/"><b>2.6.2</b></a></td>
    <td>Number of users with <a href="tools-tips/fisma-def"> privileged local system accounts.</a> (from 2.6.1) are accessible through the Agency’s network in which the privileged user is required to authenticate to the network through the <a href="tools-tips/searchad-piv"> machine-based or user-based enforcement</a> of a two-factor <a href="tools-tips/fisma-def"> PIV </a> credential or other NIST 800-63 r3 IAL3/AAL3/FAL3 credential.</td>
  </tr>
  <tr>
    <td><a href="unpriv-mgmt/"><b>2.7.1</b></a></td>
    <td>Number of network accounts assigned to unprivileged users. (Exclude <a href="tools-tips/fisma-def"> non-user accounts</a>)</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/"><b>2.7.2</b></a></td>
    <td>Number of network accounts assigned to privileged users. (Exclude <a href="tools-tips/fisma-def"> non-user accounts</a>)</td>
  </tr>
  <tr>
    <td><a href="unpriv-mgmt/"><b>2.8.1</b></a></td>
    <td> Number of <a href="tools-tips/fisma-def"> local system accounts</a> assigned to unprivileged users.</td>
  </tr>
  <tr>
    <td><a href="priv-mgmt/"><b>2.8.2</b></a></td>
    <td>Number of <a href="tools-tips/fisma-def"> local system accounts</a> assigned to privileged users.</td>
  </tr>
  <tr>
    <td><a href="data-protect/"><b>2.9.1</b></a></td>
    <td>Number of high impact systems (from 1.1.) that require all users (100% privileged and 100% unprivileged) to authenticate through the <a href="tools-tips/searchad-piv"> machine-based or user-based enforcement</a> of a two-factor <a href="tools-tips/fisma-def"> PIV </a>  credential or other NIST 800-63 r3 IAL3/AAL3/FAL3 credential.</td>
  </tr>
  <tr>
    <td><a href="data-protect/"><b>2.9.2</b></a></td>
    <td>Number of moderate impact systems (from 1.1.) that require all users (100% privileged and 100% unprivileged) to authenticate through the <a href="tools-tips/searchad-piv"> machine-based or user-based enforcement</a> of a two-factor <a href="tools-tips/fisma-def"> PIV </a>  credential or other NIST 800-63 r3 IAL3/AAL3/FAL3 credential.</td>
  </tr>
  <tr>
    <td><a href="data-protect/"><b>2.9.3</b></a></td>
    <td>Number of low impact systems (from 1.1.) that require all users (100% privileged and 100% unprivileged) to authenticate through the <a href="tools-tips/searchad-piv"> machine-based or user-based enforcement</a> of a two-factor <a href="tools-tips/fisma-def"> PIV </a>  credential or other NIST 800-63 r3 IAL3/AAL3/FAL3 credential.</td>
  </tr>
</table>
</body>
</html>

Data collected from these metrics can help your agency prioritize and guide decisions around resource allocation to assure ICAM Program effectiveness. The ultimate goal of these metrics is to enable your agency to ensure the right people have the right access to the right data at the right time. ICAM program advancement is an incremental process and unique to each agency’s mission and business needs.

The GSA FICAM Program has worked with DHS, OMB, and others to develop practical guidance to help your agency collect the data for the ICAM-related FISMA metrics. This guidance is intended to help you logically navigate and interpret the metrics to decrease your reporting time and increase usability and understanding. We hope that senior leadership will have a better “apples-to-apples” comparison across agencies if all agencies have a clearer understanding of what the metrics represent and how to collect and report them.  
