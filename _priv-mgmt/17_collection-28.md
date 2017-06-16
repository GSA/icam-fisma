---
layout: default
title: Collecting Metrics 2.5.1 & 2.5.2
permalink: priv-mgmt/collection-251-252
collection: priv-mgmt
---
>![Calculator logo](../img/calc.png){:style="width:5%;"}

1. Identify the characteristics that make your agency’s network accounts privileged.
> These will be the same characteristics you identified in Step 1 of [Metric 2.7](collection-25-27). You can find examples in [Privileged Accounts and Users](main-priv) and [FISMA Definitions](definitions).
2. Search the user repository (Active Directory) for accounts with the values identified in Step 1.
> See the [Tools & Tips](../tools-tips/searchAD) section for examples of techniques to search Active Directory.\\
If you have a good way of directly identifying non-user privileged network accounts, for example a naming convention or group, this may speed up the process. 
3. Since we’re looking for non-user accounts, exclude the accounts you identified in [Metric 2.7](collection-25-27).
4. Count the remainder and record the number for Metric 2.8.
