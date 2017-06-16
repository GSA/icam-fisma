---
layout: default
title: Definition of Privileged Account Metrics
permalink: priv-mgmt/defined-25-27
collection: priv-mgmt
---
>![Chart logo](../img/graph.png){:style="width:8%;"}

| 2.7. | Number of privileged network accounts assigned to users. (Exclude unprivileged network accounts and non-user accounts.)
| 2.7.1 | Number of privileged shared network accounts. (Exclude unprivileged network accounts and non-user accounts.)
| 2.7.2 | Number of individual users assigned to privileged shared network accounts (from 2.7.1.)
| 2.5. | Number of users with privileged network accounts. (Exclude unprivileged network accounts and non-user accounts.)

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why is Metric 2.7.2 important?</H4>
    Shared accounts generally have less accountability associated than non-shared accounts. Privileged shared accounts run a higher risk to an organization since their compromise might not be noticed as quickly.</p> 
</div>
</div>
####Privileged User Authentication
| 2.5.1 | Number of users (from 2.5) technologically required to log onto the network with a two-factor PIV card or other NIST Level of Assurance (LOA) 4 credential.
| 2.5.2| Number of users (from 2.5) allowed to use username and password as their primary method for network authentication.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why are Metrics 2.5.1 and 2.5.2 important?</H4>
    It is important to authenticate credentials when a user accesses a new network. Additionally, users must use PIV to log onto the networks to mitigate attacks such as Pass the Hash.</p> 
</div>
</div>
