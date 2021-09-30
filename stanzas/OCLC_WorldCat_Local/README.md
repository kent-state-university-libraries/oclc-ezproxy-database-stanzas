# OCLC WorldCat Local
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/OCLC_WorldCat_Local](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/OCLC_WorldCat_Local) **

## Some of OCLC's notes for this stanza

This site employs TLS 1.2. EZproxy 6.2.2 is required to proxy this resource.

Substitute your institution's domain name wherever YourInstitution is located above.

Note: The FirstSearch database stanza must be part of your config.txt file in order for the WorldCat Local definition to function properly

For WMS libraries, WorldCat Local requires the use of this stanza in place of the one above in config.txt/ezproxy.cfg:

Note: Substitute your institution's domain name wherever YourInstitution is located above. The ^A, and ^s character sequences are needed as part of the definition above and are valid syntax. For example, if your WorldCat URL is myschool.worldcat.org, then substitute myschool for all occurrences of YourInstitution in the definition above.

This configuration must be before any other configuration statements for worldcat.org.

The FirstSearch database stanza must be part of your config.txt/ezproxy.cfg file in order for the WorldCat Local definition to function properly.

&nbsp;
