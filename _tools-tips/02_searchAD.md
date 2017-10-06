---
layout: default
title: Searching Active Directory
permalink: tools-tips/searchAD
collection: tools-tips
---
---
![book logo](../img/book.png){:style="width:100px;float:right;padding-left:20px;"}

**Using The GUI** <br>
You can use the find command in *Active Directory Users and Groups* application to search for network users and groups. This interface allows you to inspect groups and group membership individually.

**PowerShell** <br>
PowerShell commands can be used to find members of administrative groups and members of child groups for the domain. Here’s an example command to list the members of a group for the example.gov domain: <br>
> dsget group "CN=Domain Admins,CN=Users,DC=example,DC=gov" -members <br>

>Sample results: <br>
> "CN=Test Admin,CN=Users,DC=example,DC=gov" <br>
> "CN=Administrator,CN=Users,DC=example,DC=gov" <br>

Other scripts can be created to search Active Directory for membership to many groups at once. Active Directory understands LDAP filters. Here is an example script to find accounts who are part of one or both of the identified groups. It also takes into consideration only users with -admin at the end of their username.
>$DomainsAdminsDn = (Get-ADGroup 'Domain Admins').DistinguishedName
>$AdminsDn = (Get-ADGroup 'Administrators').DistinguishedName
>Get-ADUser -LDAPFilter "(&(SamAccountName=*-admin) (|(memberof=$DomainsAdminsDn)(memberof=$AdminsDn)))"

To count the resulting objects instead of listing them, add this to the end of the Get-ADUser command:*-

> -ResultSetSize $null \| Measure-Object

This command uses variables to improve the readability of the filter. If you want to use the filter above in the GUI, from the find dialog, choose “Custom Search” and “Advanced”. You can’t use variables in there like in PowerShell, so make sure you use the full DN of the group.

Here are some references to help to identify built-in Windows (Active Directory) groups:

[https://technet.microsoft.com/en-us/library/cc978401.aspx](https://technet.microsoft.com/en-us/library/cc978401.aspx)

[https://support.microsoft.com/en-us/kb/243330](https://support.microsoft.com/en-us/kb/243330)
