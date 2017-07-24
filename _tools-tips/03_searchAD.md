---
layout: default
title: Searching Active Directory
permalink: tools-tips/searchAD
collection: tools-tips
---
#### Using The GUI
You can use the find command in Active Directory Users and Groups application to search for network users and groups. This interface allows you to inspect groups and group membership individually.

#### PowerShell
PowerShell commands can be used to find members of administrative groups and members of child groups for the domain. Here’s an example command to list the members of a group for the example.gov domain:
>dsget group "CN=Domain Admins,CN=Users,DC=example,DC=gov" -members
    
>Sample results:
>>"CN=Test Admin,CN=Users,DC=example,DC=gov"
>>"CN=Administrator,CN=Users,DC=example,DC=gov"

Other scripts can be created to search Active Directory for membership to many groups at once. Active Directory understands LDAP filters. Here is an example script to find accounts who are part of one or both of the identified groups. It also takes into consideration only users with -admin at the end of their username.
>$DomainsAdminsDn = (Get-ADGroup 'Domain Admins').DistinguishedName
>$AdminsDn = (Get-ADGroup 'Administrators').DistinguishedName
>Get-ADUser -LDAPFilter "(&(SamAccountName=*-admin)(|(memberof=$DomainsAdminsDn)(memberof=$AdminsDn)))"

This command uses variables to improve the readability of the filter. If you want to use the filter above in the GUI, from the find dialog, choose “Custom Search” and “Advanced”. You can’t use variables in there like in PowerShell, so make sure you use the full DN of the group.

Here are some references to help to identify built-in Windows (Active Directory) groups:

[https://technet.microsoft.com/en-us/library/cc978401.aspx](https://technet.microsoft.com/en-us/library/cc978401.aspx)

[https://support.microsoft.com/en-us/kb/243330](https://support.microsoft.com/en-us/kb/243330)

## How do I know if accounts are required to login with their PIV?
You can use LDAP filters to search Active Directory for accounts that do or don’t enforce PIV to log onto networks. Here’s an example filter that you can use in a PowerShell script or Active Directory advanced search to find users based on User Account Control – Smart Card Login Enforced on The User:

To find users where the Smart Card Login is enforced on person objects:

(&(objectCategory=person)(userAccountControl:1.2.840.113556.1.4.803:=262144))

To find users where the Smart Card Login is not enforced on person objects:

(&(objectCategory=person)(!userAccountControl:1.2.840.113556.1.4.803:=262144))

**Machine Based Enforcement (MBE):** The user is required to use their PIV credential to authenticate to each device where the policy is applied.

**User Based Enforcement (UBE):** The user is required to use their PIV credentials to authenticate to all networks and devices. Your users no longer have passwords for the network.


More details on User Account Control LDAP filters can be found here:

[https://blogs.msdn.microsoft.com/muaddib/2008/10/08/how-to-query-individual-properties-of-the-useraccountcontrol-active-directory-user-property-using-ldap/](https://blogs.msdn.microsoft.com/muaddib/2008/10/08/how-to-query-individual-properties-of-the-useraccountcontrol-active-directory-user-property-using-ldap/)

More info on AD Queries can be found here: 

[http://social.technet.microsoft.com/wiki/contents/articles/5392.active-directory-ldap-syntax-filters.aspx](http://social.technet.microsoft.com/wiki/contents/articles/5392.active-directory-ldap-syntax-filters.aspx)
