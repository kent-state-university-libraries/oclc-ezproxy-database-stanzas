# Oxford Journals
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/oxfordjournals.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/oxfordjournals.en.html) **

## Some of OCLC's notes for this stanza

October 2016: Oxford Journals will be migrating to a new platform from mid-November 2016 through January 2017. To accommodate the new platform, you will need to have an SSL certificate configured for your EZproxy server and add the new stanza below to your config.txt file.

All lines referencing the older subdomain URLs (e.g. abbs.oxfordjournals.org) and your existing Oxford Journals stanza should be maintained until migration is complete and you have an opportunity to update all starting point URLs for these resources.

Oxford Journals requires SSL configuration and the following database stanza in config.txt:

Title Oxford Journals (new platform Fall 2016)
 URL https://academic.oup.com/
 DJ oup.com

OCLC has partially tested this stanza and will continue to test during migration. Any necessary updates will be made following migration. The stanza has been tested by OUP with a small group of EZproxy users.
