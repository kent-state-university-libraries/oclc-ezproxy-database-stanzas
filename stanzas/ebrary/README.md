# ebrary
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/ebrary.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/ebrary.en.html) **

## Some of OCLC's notes for this stanza

ebrary has two options for remote access - Single-Sign-On or Patron Login + EZproxy. Add the database stanza that corresponds with your method.

ebrary single-sign-on requires the following database stanza in config.txt :

Replace YOUREBCENTRALSITE with the YOUREBECENTRALSITE name provided by ProQuest. If you have questions about this, please contact ProQuest support.

ebrary patron login + EZproxy requires the following database stanza in config.txt :

Replace YOUREBCENTRALSITE with the YOUREBCENTRALSITE name provided by ProQuest. If you have questions about this, please contact ProQuest support.

ebrary is now part of the Proquest Ebook Central platform. If you are migrating from an existing ebrary site to the new platform, please follow the instructions below. If you are a new Ebook Central subscriber, please see the new stanza on Ebook Central.

If you have an existing subscription to EBRARY that is being migrated to the Ebook Central site, first determine which migration method is appropriate for your migration based on the headers and details below, then follow those steps.

Use this method if you have a stanza like the legacy single-sign-on configuration below in your config.txt file. This option will allow users to access ebrary and their personal libraries by clicking on your proxied links. They will not have to sign in to access their saved items and bookshelves.

Note: If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.
 

Use this option is you currently have either of the legacy non-single-sign-on stanzas in your config.txt file. With this method, your users access ebrary through EZproxy and then must sign in using their ebrary credentials to access their personal bookshelf and saved items. By upgrading to SSO, users will automatically be taken directly to their personal bookshelf and see all saved items.

Note: When using the single-sign-on configuration with ebrary, EZproxy will pass your users' username to ebrary during authentication due to the Option ebraryUnecodedTokens directive. The username is considered in some cases to be personally identifiable information (PII).

Note: If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.

If you will continue to use EZproxy to allow patrons to access Ebook Central and require them to sign in with a separate Ebook Central username and password to access their personal bookshelves, use the following method.

Note: If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.
 

Note: When using the single-sign-on configuration with ebrary, EZproxy will pass your users' username to ebrary during authentication due to the Option ebraryUnecodedTokens directive. The username is considered in some cases to be personally identifiable information (PII).

To activate ebrary Single-Sign-On User Authentication:

User authentication method requirements

To maintain persistent identifiers, EZproxy requires unique user login information, and most EZproxy user authentication methods provide such information. AutoLoginIP and referring URL are incompatible since they do not provide unique user information.

Sites that use CGI authentication should insure that they are providing "loguser" information to associate distinct user information. See CGI Authentication for more information, including reference scripts for implementing CGI authentication.
