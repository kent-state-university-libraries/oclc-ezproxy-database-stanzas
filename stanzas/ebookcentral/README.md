# Ebook Central
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/ebookcentral.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/ebookcentral.en.html) **

## Some of OCLC's notes for this stanza

The stanzas on this page are intended for new Ebook Central customers only. If you are migrating to Ebook Central from EBL or ebrary, please see the EBL or ebrary stanza pages, respectively.

Ebook Central has two options for remote access - Single-Sign-On or Patron Login + EZproxy. Please confirm which method you are using with ProQuest Support, and add the database stanza that corresponds with your method.

Single-Sign-On: This option will allow users to access Ebook Central and their personal libraries by signing in to EZproxy. They will not have to sign in to a separate account on Ebook Central to access their saved items and bookshelves.

Patron Login + EZproxy: This option uses EZproxy to allow patrons to access Ebook Central and requires them to sign in with a separate Ebook Central username and password to access their personal bookshelves.

Either remote access method requires SSL configuration.

Ebook Central single-sign-on requires the following database stanza in config.txt :

Replace YOURSITE with the YOURSITE name provided by ProQuest. If you have questions about this, please contact ProQuest support.

Please note that EZproxy's AutoLoginIP directive may not be used in combination with this stanza. The stanza must also be placed above any ExcludeIP directives in config.txt.

ebrary patron login + EZproxy requires the following database stanza in config.txt :

Replace YOURSITE with the YOURSITE name provided by ProQuest. If you have questions about this, please contact ProQuest support.

NOTE: You will need to pre-proxy the URL in the 856 field of your Ebook Central MARC records.

If you are migrating to Ebook Central from an existing EBL or ebrary subscription, please see the EBL or ebrary stanza page for migration details.
 

 

 
