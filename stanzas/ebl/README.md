# EBL
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/ebl.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/ebl.en.html) **

## Some of OCLC's notes for this stanza

EBL has two options for remote access - Single Sign On or Patron Login + EZproxy. Add the database stanza that corresponds with your method.

EBL single sign on requires the following database stanza in config.txt :

Replace YOURSITE with the YOURSITE name provided by ProQuest. If you have questions about this, please contact ProQuest support.

EBL patron login + EZproxy requires the following database stanza in config.txt :

Replace YOURSITE with the YOURSITE name provided by ProQuest. If you have questions about this, please contact ProQuest support.

If you have an existing subscription to EBL that is being migrated to the Ebook Central site, first determine if you are using Single Sign On or Patron Login + EZproxy, then follow the steps for that option.

Use this option if you were using a shared secret as part of your stanza for EBL. With this setup, your users are automatically signed in to their personal accounts when they access EBL through EZproxy and can create and save bookshelves.

Note: If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.

Use this option if your users must log in to EBL after they access the site through EZproxy.

Note: If you use the kb to manage your MARC records for ProQuest ebooks, make sure you DO NOT remove the old stanza until 14 days after your migration date. This will keep redirects functioning until enough time has passed to ensure that you have updated your local MARC records to point to the new platform. After your MARC records have been updated, you can remove the old stanza. If you have questions contact OCLC Support.

This stanza must be kept in place along with your new stanza until migration is complete to ensure continued access to all of your subscribed resources.

In this example, astringyoupick is used to encrypt the user information you send to EBL. This string can be a series of numbers, letters and/or characters of your choosing. Be sure to also replace YOURSITE with your unique identifier provided to you by EBL.

Replace ####____#### with the password provided by EBL.

EBL requires a unique and consistent identifier, which can be provided via the EZproxy system. For this reason, EZproxy should be configured to appear for both on and off-campus users accessing EBL resources for the first time in a session. Often times, this requires moving the EBL stanza above any ExcludeIP (E) lines or after any Include (I) directive.
