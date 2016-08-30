# ebrary
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/ebrary.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/ebrary.en.html) **

## Some of OCLC's notes for this stanza

Note: When using the single-sign-on configuration with ebrary, EZproxy will pass your users' username to ebrary during authentication due to the Option ebraryUnecodedTokens directive. The username is considered in some cases to be personally identifiable information (PII).
 

To activate ebrary Single-Sign-On User Authentication:

Add the following stanza to config.txt :

replacing xxxxx with your ebrary site name.

It is very important that you back up the ezproxy.tkn file on a regular basis; see the section below.

If you are switching from ebrary proxy access to Single-Sign-On, existing user created ebrary bookshelves will need to be migrated to the new automatic bookshelves, ebrary Customer Support will provide additional information.
