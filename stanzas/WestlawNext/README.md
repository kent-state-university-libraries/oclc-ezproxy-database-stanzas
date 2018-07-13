# WestLawNext
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/westlawnext.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/westlawnext.en.html) **

## Some of OCLC's notes for this stanza

WestLawNext requires the following database stanza in config.txt :

Replace "YOURSPONSORSHIP" with the code provided specifically for your institution by Westlaw.

# if Option X-Forwarded-For is above this, then include:
 
 Option NoX-Forwarded-For
 
 # If using recommended wildcard certificate, then include:
 
 Option HttpsHyphens
 
 # Some schools also need to add the following: (try it with or with out the https:// pre-append)
 
 H https://1.next.westlaw.com
