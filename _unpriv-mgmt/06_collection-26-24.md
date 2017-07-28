---
layout: default
title: Collecting Metrics 2.6, 2.6.1, 2.6.2, 2.4
permalink: unpriv-mgmt/collection-26-24
collection: unpriv-mgmt
---
## Unprivileged User Authentication
>![Calculator logo](../img/calc.png){:style="width:5%;"}

1. Identify the characteristics that make your agency’s network accounts privileged. We’ll exclude those accounts from this metric.
> • See the [FISMA Definitions](../tools-tips/definitions) and [Additional Information](../priv-mgmt/main-priv#how-do-i-find-privileged-accounts) pages for examples of these characteristics. They are typically Groups in Active Directory.
2. Search for and exclude accounts with the values identified in Step 1.
> • See slides 5 and 6 for example searches.
3. Count the remaining accounts that are assigned to/ used by individual people and record number for Metric 2.6.
4. Now, count the number of accounts that are shared by 2 or more people and record number for Metric 2.6.1.
> • See the [Additional Information](../priv-mgmt/main-priv#how-do-i-find-privileged-accounts) page for examples of shared accounts.
5. Of the accounts identified in Step 4, count the number of unique people with access to these accounts and record number for Metric 2.6.2. You might need to contact the point of contact for the account to research this information.
6. Of the accounts identified in Step 3, identify the number of users of the accounts. Take care to eliminate duplicates from the count if two accounts are researched and identified to be assigned to the same person. Record this number for Metric 2.4.![Recycle logo](../img/recycle.png){:style="width:5%;"}

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Beware!</H4>
    John.smith.1 and john.smith.2 might both belong to the same person!</p> 
</div>
</div>

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Save the result from Metric 2.5 (Step 6)!</H4>
    You'll use the user information found here again for the next two metrics.</p> 
</div>
</div>
