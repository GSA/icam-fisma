---
layout: default
title: Collecting Metrics 2.6, 2.6.1, & 2.6.2
permalink: unpriv-mgmt/collection-26-262
collection: unpriv-mgmt
---
## Network Accounts
>![Calculator logo](../img/calc.png){:style="width:5%;"}

**_Where Do I Start?_**

1. Identify the characteristics that make your agency’s network accounts privileged. We’ll exclude those accounts from this metric.
> • See the [FISMA Definitions](../tools-tips/definitions) and [Additional Information](../priv-mgmt/main-priv/add-info) pages for examples of these characteristics. They are typically Groups in Active Directory. Some agencies also have account naming conventions.
2. Search for and exclude accounts with the values identified in Step 1.
> • See pages 5 and 6 for example searches. We're looking for non-admin (unprivileged) accounts.
3. Count the accounts in step 2 that are assigned to/used by individual people (non-system) and record number for Metric 2.6.1.
> • See page 5 for an example of how to count objects using PowerShell.       
4. Search for and include accounts with the values identified in Step 1.
> •See pages 5 and 6 for example searches. We’re looking for admin (privileged) accounts.
5. Count the accounts in step 4 that are assigned to/used by individual people (non-system) and record number for Metric 2.6.2.
> • See page 5 for an example of how to count objects using PowerShell.

![light bulb logo](../img/ahabrn.png){:style="width:5%;"}
<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text">
    John.smith.1 and john.smith.2 might both belong to the same person!</p>
</div>
</div>

![recycle logo](../img/recycle.png){:style="width:5%;"}
<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Save for Later!!</H4>
    You'll use the user information found here again for the next two metrics.</p>
</div>
</div>
