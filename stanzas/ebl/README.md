# EBL
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/ebl.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/ebl.en.html) **

## Some of OCLC's notes for this stanza

EBL customers are being upgraded to Ebook Central, which requires SSL configuration and EZproxy 6.2.2.

Please add these additional lines:

Please note that EZproxy's AutoLoginIP directive may not be used in combination with this stanza. The stanza must also be placed above any ExcludeIP directives in config.txt.

Continue to use your existing starting point URLs until ProQuest confirms migration is complete. At this time, you can update your starting point URLs to include target URLs from the new Ebook Central stanza added.
