---
layout: default
title: Collecting Metrics 2.16 & 2.17
permalink: pacs/collection-216-217
collection: pacs
---
## PACS Procurement Compliance & PIV Enforcement
>![Calculator logo](../img/calc.png){:style="width:5%;"}

1. Work with your agency’s Physical Security personnel to identify all perimeter and sensitive area access readers across all locations in your agency.
2. Identify each instance of a PACS validation system in use across the agency.
3. Validate that the product's (readers and validation software) comply with [NIST FIPS 201](http://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.201-2.pdf). Compliant products are listed on the [GSA Approved Products List (APL)](https://www.idmanagement.gov/approved-products-list/). Hardware and software versioning and other specific information can be found inside the Approved Letters on the APL. Only the exact versions of hardware and software listed are compliant.
>• See the [PACS Resources Section](#additional-information)  for sample steps to check for compliance.\
4. Determine which validation system is configured for each compliant reader. Count the number of readers that comply, divide by the total number of readers the agency has across all locations and multiply by 100 to obtain the percentage for this metric. Record this number for Metric 2.16.
5. Of the readers identified in Step 3, count the number that are configured to utilize the PKI (either Card Authentication or PIV Authentication Key Certificate) for routine access.
6. Divide Step 4 by the total number from Step 1, and multiply by 100 to obtain the percentage for this metric. Record this number for Metric 2.17.

## Additional Information 
>![Magnifying Glass logo](../img/focus.png){:style="width:5%;"}

How do I look through my PACS software in an HID Validation Solution Environment?

1. Create an excel based inventory of all readers for a “given area”.
> • Take note of the make, model, hardware revision, and firmware revision\\
> • Take note of whether the above matches what is listed on the APL\
2. Determine/Confirm which validation system is configured to support the reader
> • Log into pivCLASS PACS Services Server\\
> • Open pivCLASS PACS Service Administration Application, log in if necessary\\
> • Go to Tools > Configure PACS Service\\
> • Click the Reader Services Tab\\
> • In the left panel, expand the “Panels” tree\\
> • For each PAM panel configured: (1) Match the readers therein to the readers inventoried above, and (2) note which Assurance profile the reader is configured.\\
> • Write this information on the Inventory Report.

<div class="usa-alert usa-alert-info">
  <div class="usa-alert-body">
    <p class="usa-alert-text"><H4>Need More Information?</H4>
    • <a href="https://www.idmanagement.gov/approved-products-list/">FIPS 201 Approved Products List]</a><br>
    • <a href="https://georgewbush-whitehouse.archives.gov/omb/memoranda/fy2006/m06-18.pdf">OMB M-06-18</a><br>
    • <a href="https://www.dhs.gov/sites/default/files/publications/ISC_Risk-Management-Process_Aug_2013.pdf">DHS ISC Risk Management Process</a></p> 
</div>
</div>

*If you use a different vendor’s validation system, and are not sure how to collect these metrics, please email icam@gsa.gov for assistance.*
