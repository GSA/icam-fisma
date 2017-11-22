---
layout: default
title: Section Resources
permalink: /priv-mgmt/section-resources
collection: priv-mgmt
---
---

### How do I find Privileged Accounts? ![focus logo](../img/focus.png){:style="width:50px;float:right;"}


**_By Name:_** Your agency may have a naming convention for its accounts to identify privileged users.

<i>For example,</i> some names may have -admin or -domainadmin as part of their usernames (jdoe-admin). This shouldn’t be the only way to find administrators since access can change over time.

**_By Privileges:_** Privileged network accounts have elevated access rights, typically in Active Directory, accounts are added to groups. Look through Active Directory to identify the groups that grant elevated permissions.

**_By Inspection:_** Occasionally, accounts are assigned elevated privileges individually. You will need to know your user population and find the fringe cases.

Take care to remove duplicate accounts from the results! These metrics are counting unique accounts and users. For more information on assurance levels, refer to <a href="https://doi.org/10.6028/NIST.SP.800-63-3">NIST SP 800-63-3.</a>

**_Examples:_** <br>
For most agencies, network accounts are managed in Active Directory. Examples of shared accounts are accounts used for helpdesk, test, and training or guest accounts.
