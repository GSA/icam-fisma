---
layout: default
title: Privileged Accounts and Users
permalink: priv-mgmt/main-priv
collection: priv-mgmt
---
This section covers FISMA metrics around privileged accounts and users (2.7, 2.7.1, 2.7.2, 2.5, 2.5.1, 2.5.2, 2.8, 2.9, 2.10, 2.11 and 2.12) 

>![Chart logo](../img/graph.png){:style="width:8%;"}

### [Privileged Network Accounts & Users](collection-25-27)

| 2.7. | Number of privileged network accounts assigned to users. (Exclude unprivileged network accounts and non-user accounts.)
| 2.7.1 | Number of privileged shared network accounts. (Exclude unprivileged network accounts and non-user accounts.)
| 2.7.2 | Number of individual users assigned to privileged shared network accounts (from 2.7.1.)
| 2.5. | Number of users with privileged network accounts. (Exclude unprivileged network accounts and non-user accounts.) ![Chart logo](../img/recycle.png){:style="width:3%;"}

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why is Metric 2.7.2 important?</H4>
    Shared accounts generally have less accountability associated than non-shared accounts. Privileged shared accounts run a higher risk to an organization since their compromise might not be noticed as quickly.</p> 
</div>
</div>

### [Privileged User Authentication](collection-251-252)

| 2.5.1 | Number of users (from 2.5) technologically required to log onto the network with a two-factor PIV card or other NIST Level of Assurance (LOA) 4 credential.
| 2.5.2| Number of users (from 2.5) allowed to use username and password as their primary method for network authentication.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why are Metrics 2.5.1 and 2.5.2 important?</H4>
    It is important to authenticate credentials when a user accesses a new network. Additionally, users must use PIV to log onto the networks to mitigate attacks such as Pass the Hash.</p> 
</div>
</div>

### [Non-User Privileged Network Accounts](collection-28)

|2.8| Number of non-user privileged network accounts. (Exclude unprivileged network accounts and privileged network accounts assigned to a user.)

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why is Metric 2.8 important?</H4>
    Privileged accounts provide greater access rights than non-privileged accounts. Some of these accounts could be thought of as having the "keys to the kingdom". Although an account may be considered non-user, it may not stop someone from using it to log onto a network if compromised. Since they're not associated with a user, it is more difficult to identify accountability for the account's actions.

It is important to understand the makeup of all types of privileged accounts so you can take steps to avoid the risk of compromise.</p> 
</div>
</div>

### [Privileged User Review, Adjustments, & Termination](collection-29-210)

|2.9| Number of privileged network users (from 2.5) that had their privileges reviewed at least once in the past twelve months.
|2.10| Number of privileged network users (from 2.5) that had their privileges adjusted or terminated in the past 12 months after a review.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why are metrics 2.9 and 2.10 important?</H4>
    A user needs the correct level of access to the right resources to fulfill their job function. Reviewing and correcting access supports least privilege, and policies such as segregation of duties.</p> 
</div>
</div>

### [Users with Privileged Local System Accounts and Users Required to Use PIV/LOA 4](collection-211-212)

|2.11| Number of users with privileged local system accounts.
|2.12| Number of users with privileged local system accounts (from 2.11) technologically required to log onto the system with a two-factor PIV card or other NIST LOA 4 credential.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Why are metrics 2.11 and 2.12 important?</H4>
    <p>• Understanding this user population helps to validate that they have the appropriate access across information systems</p>
    <p>• Issuing the appropriate credentials to user populations is meaningless unless agencies are requiring the use of these credentials</p>
    </p> 
</div>
</div>
<br>
## How do I find privileged accounts?
<b> By Name: </b> Your agency may have a naming convention for its accounts to identify privileged users. For example, some names may have -admin or -domainadmin as part of their usernames (jdoe-admin). This shouldn’t be the only way to find administrators since access can change over time.

<b> By Privileges:</b> Privileged network accounts have elevated access rights, typically in Active Directory, accounts are added to groups. Look through Active Directory to identify the groups that grant elevated permissions.

<b> By Inspection: </b> Occasionally, accounts are assigned elevated privileges individually. You will need to know your user population and find the edge cases.

Take care to remove duplicate accounts from the results! These metrics are counting unique accounts and users. For more information on Levels of Assurance, refer to [NIST SP 800-63-2](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-63-2.pdf).

### Examples:
For most agencies, network accounts are managed in Active Directory. Examples of shared accounts are accounts used for helpdesk, test, and training or guest accounts.
