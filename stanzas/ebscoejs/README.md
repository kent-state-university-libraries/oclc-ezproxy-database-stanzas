# EBSCO Electronic Journals Service
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/ebscoejs.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/ebscoejs.en.html) **

## Some of OCLC's notes for this stanza

EBSCO Electronic Journals Service requires the following database stanza in config.txt :

EBSCO no longer maintains ebscoejs.txt file, so in addition to the above stanza, you will also need to include the EZproxy stanza for each full text publisher you subscribe to. You can find many on the Database Stanzas page.

Adding the entire ebscoejs.txt as an IncludeFile is no longer the suggested method for configuration of resources accessed through EBSCO Electronic Journals Service because this file contains many duplicate host statements and outdated database stanzas, for example Sage Publications and Wiley Online Library. Adding stanzas for each individual resource will ensure that you are using the most up-to-date stanza for that resource.

Including duplicate host statements in your config.txt can cause the following problems:

We will continue to make ebscoejs.txt available for reference because it contains stanzas for resources not currently published on the EZproxy Database Stanzas page. When selecting stanzas from this file for inclusion in your config.txt file, use caution and do not include multiple stanzas containing duplicate URL, Host, HJ, Domain, and DJ lines. You only need to include these lines once, and all resources at these URLs will be accessible. For more information about when to include a new stanza and when to use one that already exists, see Starting Point URLs & config.txt.
