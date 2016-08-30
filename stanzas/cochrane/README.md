# Cochrane Library
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/cochrane.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/cochrane.en.html) **

## Some of OCLC's notes for this stanza

The following configuration is required for Cochrane Library:

If you find that the Cochrane Library site does not work correctly with the above configuration, use the following alternative configuration, including the directive "HTTPHeader X-Requested-With".

If your config.txt file contains stanzas for both Cochrane Library and Wiley Online Library, make sure that the Cochrane Library stanza follows the Wiley Online Library stanza. This will ensure that processing of the Wiley Online Library stanza includes all processing directives in that stanza but will not interfere with the processing of the Cochrane Library stanza.
 
