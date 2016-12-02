# SAGE Publications
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/sage.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/sage.en.html) **

## Some of OCLC's notes for this stanza

December 2016: Sage is in the process of migrating to a new platform. The new site’s URL patterns are much simpler, and ultimately will eliminate the need for the lengthy sage.txt IncludeFile.

At your earliest convenience, please add the new stanza below the current one (either the IncludeFile line or your local Sage stanza):

HTTPHeader X-Requested-With
 Title Sage Journals
 URL http://journals.sagepub.com
 HJ businessresearcher.sagepub.com
 HJ www.sagepub.co.uk
 HJ data.sagepub.com
 HJ sk.sagepub.com
 HJ library.cqpress.com
 HJ uk.sagepub.com
 HJ methods.sagepub.com
 HJ widgets.twimg.com
 HJ brightcove.com
 DJ sagepub.com
 DJ sagepub.co.uk
 DJ cqpress.com
 DJ widgets.twimg.com
 DJ brightcove.com
 Find url = "http://
 Replace url = "http://^A
 Find "google-analytics.com
 Replace "^pgoogle-analytics.com^
 Find url = document.location.protocol + "//" + document.location.host
 Replace url = "http://journals.sagepub.com/"

Sage has requested that libraries not begin updating their Starting Point URLs until Tuesday December 6. Permanent redirects will be in place from the old URLs (e.g. aaf.sagepub.com) to the new platform to assure continued access during the transition period.

The previous stanza information for Sage Publications is below.

A configuration file for SAGE Publications that includes all of the SAGE journal hostnames is available for download. 
 

Once downloaded, save this file in your EZproxy directory and include the following line as the last line in your EZproxy config.txt :

Whenever you download a new version of the sage.txt file and replace the old file in your EZproxy directory, make sure to restart your EZproxy server for the changes to take effect.
 
