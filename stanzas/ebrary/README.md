# ebrary
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/ebrary.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/ebrary.en.html) **

## Some of OCLC's notes for this stanza

ebrary customers are being upgraded to Ebook Central, which requires SSL configuration and EZproxy 6.2.2.

If you have EBL (in addition to ebrary), please see the EBL stanza page for migration details.

If you have ebrary only (no EBL), first determine if you are using Single Sign On or Patron Login + EZproxy, then follow the steps for that option.

Single-Sign-On: This option will allow users to access Ebook Central and their personal libraries by signing in to EZproxy. They will not have to sign in to a separate account on Ebook Central to access their saved items and bookshelves.

Patron Login + EZproxy: This option uses EZproxy to allow patrons to access Ebook Central and requires them to sign in with a separate Ebook Central username and password to access their personal bookshelves.

This option will allow users to access Ebook Central and their personal libraries by signing in to EZproxy. They will not have to sign in to a separate account on Ebook Central to access their saved items and bookshelves.

This stanza can be added any time prior to your upgrade, and it will not interfere with your existing ebrary access.
 

Note: If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.

With your current method, your users access ebrary through EZproxy and then must sign in using their ebrary credentials to access their personal bookshelf and saved items.

By upgrading to SSO, users will automatically be taken directly to their personal bookshelf and see all saved items. Note: When using the single-sign-on configuration with ebrary, EZproxy will pass your users' username to ebrary during authentication due to the Option ebraryUnecodedTokens directive. The username is considered in some cases to be personally identifiable information (PII).

Note: If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.

If you will continue to use EZproxy to allow patrons to access Ebook Central and require them to sign in with a separate Ebook Central username and password to access their personal bookshelves, use the following method.

Replace YOUREBCENTRALSITE with the Ebook Central site ID included in your migration paperwork.

Note: If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.

You will also need to pre-proxy the URL in the 856 field of your Ebook Central MARC records.
