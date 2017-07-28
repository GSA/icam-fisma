---
layout: default
title: Collecting Metric 2.8
permalink: priv-mgmt/collection-28
collection: priv-mgmt
---
## Non-User Privileged Network Accounts
>![Calculator logo](../img/calc.png){:style="width:5%;"}

1. Identify the characteristics that make your agency’s network accounts privileged.
> •  These will be the same characteristics you identified in Step 1 of [Metric 2.7](collection-25-27). You can find examples on the [FISMA Definitions](../tools-tips/definitions) and [Additional Information](../priv-mgmt/main-priv#how-do-i-find-privileged-accounts) pages.
2. Search the user repository (Active Directory) for accounts with the values identified in Step 1.
> •  See the [Tools & Tips](../tools-tips/searchAD) section for examples of techniques to search Active Directory.\\
•  If you have a good way of directly identifying non-user privileged network accounts, for example a naming convention or group, this may speed up the process. 
3. Since we’re looking for non-user accounts, exclude the accounts you identified in [Metric 2.7](collection-25-27).
4. Count the remainder and record the number for Metric 2.8.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Step 4 Example</H4>
    If there are 100 privileged accounts identified in Step 2 and 90 accounts identified in metric 2.7, the total privileged, non-user privileged network accounts is 10.</p> 
</div>
</div>
