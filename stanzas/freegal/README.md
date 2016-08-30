# Freegal Music Service
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/freegal.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/freegal.en.html) **

## Some of OCLC's notes for this stanza

Freegal Music Service requires that the last two lines of config.txt  are:

where somesecret and site are both provided to you by Freegal.

To access Freegal, you will need to construct a URL similar to:

replacing ezproxy.yourlib.org:2048 with your own EZproxy server hostname and port.

The IncludeIP directive forces all users to authenticate. If you omit this directive, browsers accessed by local users will go into a redirect loop.
