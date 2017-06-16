---
layout: default
title: Searching Active Directory - PIV
collection: tools-tips
permalink: tools-tips/searchAD-PIV/
---
## How do I know if accounts are required to login with their PIV?
You can use LDAP filters to search Active Directory for accounts that do or don’t enforce PIV to log onto networks. Here’s an example filter that you can use in a PowerShell script or Active Directory advanced search to find users based on User Account Control – Smart Card Login Enforced on The User:

To find users where the Smart Card Login is enforced on person objects:

(&(objectCategory=person)(userAccountControl:1.2.840.113556.1.4.803:=262144))

To find users where the Smart Card Login is not enforced on person objects:

(&(objectCategory=person)(!userAccountControl:1.2.840.113556.1.4.803:=262144))

**Machine Based Enforcement (MBE):** The user is required to use their PIV credential to authenticate to each device where the policy is applied.

**User Based Enforcement (UBE):** The user is required to use their PIV credentials to authenticate to all networks and devices. Your users no longer have passwords for the network.


More details on User Account Control LDAP filters can be found here:

https://blogs.msdn.microsoft.com/muaddib/2008/10/08/how-to-query-individual-properties-of-the-useraccountcontrol-active-directory-user-property-using-ldap/

More info on AD Queries can be found here: 

http://social.technet.microsoft.com/wiki/contents/articles/5392.active-directory-ldap-syntax-filters.aspx
