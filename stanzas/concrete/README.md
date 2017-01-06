# American Chemical Society
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/concrete.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/concrete.en.html) **

## Some of OCLC's notes for this stanza

The American Concrete Institute requires the following database stanza in config.txt :

Note: You must replace USERNAMEHERE with the username and PASSWORDHERE with the password.

This version targets the following Starting Point URL: http://ezproxy.yourlib.org/login?url=https://www.concrete.org/securesignin.aspx. The page will load with the username and password pre-filled.  When pressing the button to Sign In, authentication occurs and then the user ends up in a non-proxied but fully functional session as that user. 

This stanza also works if the target is a specific journal such as: http://ezproxy.yourlib.org/login?url=https://www.concrete.org/securedsignin.aspx?returnurl=%2fpublications%2facimaterialsjournal.aspx
