---
layout: default
title: Searching Active Directory - PIV
permalink: tools-tips/searchAD-PIV
collection: tools-tips
---
---
![Book logo](../img/book.png){:style="width:100px;float:right;padding-left:20px;"}

**Machine Based Enforcement (MBE):** <br>
The user is required to use their PIV credential to authenticate to each device where the policy is applied.

**User Based Enforcement (UBE):** <br>
The user is required to use their PIV credentials to authenticate to all networks and devices. Your users' Active Directory password hash values have been replaced with hash values of long (120 character) randomized strings.

**How do I know if accounts are required to login with their PIV (UBE)?** <br>
You can use LDAP filters to search Active Directory for accounts that do or don’t enforce PIV to log onto networks. Here’s an example filter that you can use in a PowerShell script or Active Directory advanced search to find users based on *User Account Control – Smart Card Login Enforced on The User.*

To find users where the Smart Card Login is enforced on person objects: <br>
(&(objectCategory=person)(userAccountControl:1.2.840.113556.1.4.803:=262144))

To find users where the Smart Card Login is not enforced on person objects: <br>
(&(objectCategory=person)(!userAccountControl:1.2.840.113556.1.4.803:=262144))


More details on User Account Control LDAP filters can be found here:
[http://social.technet.microsoft.com/wiki/contents/articles/5392.active-directory-ldap-syntax-filters.aspx](http://social.technet.microsoft.com/wiki/contents/articles/5392.active-directory-ldap-syntax-filters.aspx)

More info on AD Queries can be found here:<br>
[https://blogs.msdn.microsoft.com/muaddib/2008/10/08/how-to-query-individual-properties-of-the-useraccountcontrol-active-directory-user-property-using-ldap/](https://blogs.msdn.microsoft.com/muaddib/2008/10/08/how-to-query-individual-properties-of-the-useraccountcontrol-active-directory-user-property-using-ldap/)
