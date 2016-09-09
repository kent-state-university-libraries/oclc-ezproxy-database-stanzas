# Cambridge Core
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/cambridgecore.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/cambridgecore.en.html) **

## Some of OCLC's notes for this stanza

Cambridge Core is the new platform through which subscribers to Cambridge University Press resources can access all of their subscribed content. This single platform replaces the previous Cambridge Books Online, Cambridge Companions Online, Cambridge Journals Online, Cambridge Histories Online, Shakespeare Survey Online and University Publishing Online platforms.

Cambridge Core requires an SSL certificate, SSL configuration and the following database stanza in config.txt :

To ensure continued access to all Cambridge University Press, make sure this stanza is placed above any existing Cambridge resources stanzas. This stanza should provide access to all Cambridge resources and redirects are in place for all old URLs; however, you can retain any existing stanzas or add missing target URLs from your starting point URLs as HJ statements to the stanza above if you would like to remove the old stanzas.

Note: Thank you to Christian Wimmer, Dom Benson, and Laurence Lockton for their work developing this stanza!
 
