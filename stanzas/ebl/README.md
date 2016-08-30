# EBL
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/ebl.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/ebl.en.html) **

## Some of OCLC's notes for this stanza

EBL requires the following configuration in config.txt :

 

In this example, astringyoupick is used to encrypt the user information you send to EBL. This string can be a series of numbers, letters and/or characters of your choosing. Be sure to also replace INSTITUTION_ID with your unique identifier provided to you by EBL.

Replace ####____#### with the password provided by EBL.

EBL requires a unique and consistent identifier, which can be provided via the EZproxy system. For this reason, EZproxy should be configured to appear for both on and off-campus users accessing EBL resources for the first time in a session. Often times, this requires moving the EBL stanza above any ExcludeIP (E) lines or after any Include (I) directive.
