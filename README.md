LDAP plugin for trac
====================

This is an evolution of LdapPlugin for Trac, adding support for automatic
discovery of email addresses and support for authz-style authentication.

Config
------

The LDAP configuration works the same as the original LDAP plugin.

LDAP authz permissions require the full dn for the group, e.g.:

    [repository:*]
    "cn=repoview,ou=Groups,dc=example,dc=com" = BROWSER_VIEW
    * = 
