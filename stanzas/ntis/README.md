# National Technical Information Service (NTIS)
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/ntis](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/ntis) **

## Some of OCLC's notes for this stanza

The National Technical Information Service (NTIS) does not provide IP authentication or a simple method for username/password authentication. The following database stanza can be used to direct EZproxy to fill in your institution's username and password when it is requested by the NTIS server.

substituting your own username and password at the appropriate points.

Since both local and remote users would need to have this information provided, see AutoLoginIP for an example of how to use this directive to proxy your local users transparently when accessing this service.

If you are accessing this link through a US GPO PURL, you will also need to define the PURL service to EZproxy like this:

&nbsp;
