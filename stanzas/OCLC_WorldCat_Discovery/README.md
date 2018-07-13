# OCLC WorldCat Discovery
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/worldcatdiscovery.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/worldcatdiscovery.en.html) **

## Some of OCLC's notes for this stanza

OCLC WorldCat Discovery requires SSL Configuration and the following database stanza in config.txt :

For every [my institution] in the stanza above, insert the institution used with your WorldCat Discovery instance. For [registry_id] above, insert your institution's registry id.

Also add the following hidden stanza to allow the non-customized pieces of the IDM to be proxied as well as static scripts/images that support WorldCat Local but do not need to be customized. The URL in this stanza is irrelevant; it is only the presence of "DJ worldcat.org" that matters.
