---
layout: default
title: Collecting Metrics 2.5.1 & 2.5.2
permalink: priv-mgmt/collection-251-252
collection: priv-mgmt
---
## Privileged User Authentication
>![Calculator logo](../img/calc.png){:style="width:5%;"}

1. Start with the users identified in [Metric 2.5](collection-25-27).
2. Exclude users that can log onto the network with anything other than a PIV / LOA 4 credential. (Examples: One time password tokens, SMS PIN & Password, Username and Password).
> •  Some users have multiple accounts - *a user must be excluded if even one of their accounts lets them log onto the network with something other than a PIV / LOA4 credential.*\\
•  Users who have the option of PIV or Username/Password should also be excluded since PIV is not required.
3. For the remaining users, include users that are technologically required through user based enforcement (UBE). This requires the user to use PIV on all devices to access the network and disables the password. The users that have this enforcement should be counted. Refer to [Searching Active Directory - PIV](../tools-tips/searchAD#how-do-i-know-if-accounts-are-required-to-login-with-their-piv) for information on querying for these users.
4. For the remaining users who have a PIV but who aren’t UBE or MBE, exclude users who can log onto the network without PIV.
5. Count the total number of unique users who have not been excluded in previous steps on this slide and record number for Metric 2.5.1.
6. Start with the users identified in Step 1 and exclude the users identified in Step 5.
7. For each remaining account, does the account have the abilityto log onto the network using a username & password? If it does, the user of the account should be counted.
8. Count the total number of unique users found in Step 7 and record the number for Metric 2.5.2.
