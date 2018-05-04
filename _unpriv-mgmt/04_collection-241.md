---
layout: default
title: Collecting Metric 2.4.1
permalink: /unpriv-mgmt/collection-241
collection: unpriv-mgmt
---
---
### Unprivileged Network Users![calc logo](../img/calc.png){:style="width:40px;float:right;"}
#### Where Do I Start?

1.	Identify the characteristics that make your agency’s network accounts privileged. We'll exclude those accounts from this metric.
>•	See <a href="../priv-mgmt/section-resources">How do I find Privileged Accounts?</a> for examples of these characteristics. They are typically groups in Active Directory.

2. Search the user repository (Active Directory) for and exclude accounts with the values identified in Step 1.
>•	See <a href="../tools-tips/searchAD">Tools & Tips for Active Directory</a> or <a href="../tools-tips/searchAD-PIV ">Tools & Tips for Active Directory-PIV</a> for example searches.

3. Count the accounts in step 2 that are assigned to/ used by individual people (non-system).
>•	See <a href="../tools-tips/searchAD">Tools & Tips for Active Directory</a> for an example of how to count objects using PowerShell.    

4.	Identify the number of users of the accounts. Take care to eliminate duplicates from the count if two accounts are researched and identified to be assigned to the same person. Record this number for <b>Metric 2.4.1.</b>

![aha logo](../img/aha.png){:style="width:45px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
John.smith.1 and john.smith.2 might both belong to the same person!
</div>
</div>

![recycle logo](../img/recycle.png){:style="width:40px;float:left;"}
<style>
div .usa-alert {background-color: #e1f3f8;}
div .usa-alert-text {
padding-left: 5rem;
horizontal-align: right; }
  </style>
  <div class="usa-alert">
  <div class="usa-alert-text">
<p class="usa-alert-text"><H4>Save the result from Metric 2.4.1!</H4> You'll use the user information found here again for metrics 2.4.2, 2.4.3, and 2.4.4.</p>  
</div>
</div>
