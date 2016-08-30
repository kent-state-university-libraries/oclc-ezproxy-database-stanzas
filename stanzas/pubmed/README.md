# PubMed
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/pubmed.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/pubmed.en.html) **

## Some of OCLC's notes for this stanza

The MyNCBI feature in PubMed uses https which requires the SSL configuration on your EZproxy server.

PubMed requires the lines up to DJ static.pubmed.gov to work properly and the Find/Replace lines, although you can modify the URL line to point to your own holdings URL if relevant.

The lines between DJ static.pubmed.gov and the Find/Replace lines are for linking hosts that are used to link from PubMed to content held in licensed databases. You may omit the linking host lines if they are not relevant to your needs.

The linking lines for EBSCOhost that appeared in earlier definitions of PubMed were removed since the standard definition for EBSCOhost contains everything needed to insure that links from PubMed to EBSCOhost will be handled correctly.
