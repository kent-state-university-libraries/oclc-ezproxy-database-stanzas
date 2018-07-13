# Nexis Uni
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/nexis-uni.en.html#par_text_title](https://www.oclc.org/support/services/ezproxy/documentation/db/nexis-uni.en.html#par_text_title) **

## Some of OCLC's notes for this stanza

Nexis Uni requires EZproxy 6.1 or higher, SSL configuration and the following database stanza in config.txt. This stanza utilizes HTTPHeader behavior that was introduced in EZproxy 6.1.

Customers migrating from LexisNexis Academic to Nexis Uni must place the Nexis Uni stanza above any legacy LexisNexis stanzas in config.txt.

NOTE: The previously published version of this stanza (July 13, 2017) contained a typographical error ("X-RequestedWith" instead of "X-Requested-With"). It also contained an unnecessary "Option Cookie" directive at the bottom of the stanza.
