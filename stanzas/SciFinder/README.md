# SciFinder
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/scifinder.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/scifinder.en.html) **

## Some of OCLC's notes for this stanza

This page describes how to configure EZproxy to work with the web-based version of SciFinder. If you want to configure EZproxy to work with the SciFinder Scholar client program for Macintosh and Windows, see SciFinder Scholar.

The web-based version of SciFinder requires SSL configuration and the following configuration in config.txt :

Note: A setting that should not be used in the configuration settings is "DJ cas.org" because it is known to cause "HTTP 500 Internal Server Error" on IE and "500: Server Error" on Firefox during the SciFinder login process.

If you are having problems accessing this resource with your instance of EZproxy, try upgrading to the newest version of EZproxy here.
