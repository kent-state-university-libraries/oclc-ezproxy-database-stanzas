# Ebrary
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/ebrary](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/ebrary) **

## Some of OCLC's notes for this stanza

ebrary customers are being upgraded to Ebook Central, which requires EZproxy 6.2.2.

If you have EBL (in addition to ebrary), please see the EBL stanza page for migration details.

If you have ebrary only (no EBL), first determine if you are using Single Sign On or Patron Login + EZproxy, then follow the steps for that option.

Single-Sign-On: This option will allow users to access Ebook Central and their personal libraries by signing in to EZproxy. They will not have to sign in to a separate account on Ebook Central to access their saved items and bookshelves.

Patron Login + EZproxy: This option uses EZproxy to allow patrons to access Ebook Central and requires them to sign in with a separate Ebook Central username and password to access their personal bookshelves.

&nbsp;

This option will allow users to access Ebook Central and their personal libraries by signing in to EZproxy. They will not have to sign in to a separate account on Ebook Central to access their saved items and bookshelves.

1. Leave your existing ebrary stanza exactly as it is. Make sure it is placed before ANY ExcludeIP directives. This option is NOT compatible with AutoLoginIP lines; you cannot have any AutoLoginIP directives in config.txt if you are using this option.

2. Add the following stanza below your existing configuration, before any ExcludeIP directives. Replace YOUREBCENTRALSITE with the Ebook Central site ID contained in your migration paperwork.

This stanza can be added any time prior to your upgrade, and it will not interfere with your existing ebrary access.

3. Continue to use your existing starting point URLs until ProQuest confirms migration is complete. At this time, you can update your starting point URLs to include target URLs from the new Ebook Central stanza added in step three.

Note:&nbsp;If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.

&nbsp;

With your current method, your users access ebrary through EZproxy and then must sign in using their ebrary credentials to access their personal bookshelf and saved items.

By upgrading to SSO, users will automatically be taken directly to their personal bookshelf and see all saved items. Note:&nbsp;When using the single-sign-on configuration with ebrary, EZproxy will pass your users' username to ebrary during authentication due to the Option ebraryUnecodedTokens directive. The username is considered in some cases to be personally identifiable information (PII).

1. Leave your existing ebrary stanza in config.txt, though it must be moved above any ExcludeIP statements if it is not already.

2. Contact ebooksupport@proquest.com to let them know you would like to use the SSO configuration with your new Ebook Central site. SSO will not work unless ProQuest has made the necessary changes to your site configuration.

3. Add the following stanza to your config.txt file making sure it is placed before any ExcludeIP directives. This option is NOT compatible with AutoLoginIP lines; you cannot have any AutoLoginIP directives in config.txt if you are using this option. Replace YOUREBCENTRALSITE with the Ebook Central site ID contained in your migration paperwork.

4. Continue to use your existing starting point URLs until ProQuest confirms migration is complete. At this time, you can update your starting point URLs to include target URLs from the new Ebook Central stanza added in step three.

Note:&nbsp;If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.

&nbsp;

If you will continue to use EZproxy to allow patrons to access Ebook Central and require them to sign in with a separate Ebook Central username and password to access their personal bookshelves, use the following method.

1. Leave your existing ebrary stanza as is. It can be placed anywhere in config.txt.

2. Add the following stanza below your existing ebrary stanza.

Replace YOUREBCENTRALSITE with the Ebook Central site ID included in your migration paperwork.

3. Continue to use your existing starting point URLs until ProQuest confirms migration is complete. At this time, you can update your starting point URLs to include target URLs from the new Ebook Central stanza added in step two.

Note: If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support

You will also need to pre-proxy the URL in the 856 field of your Ebook Central MARC records.

&nbsp;
