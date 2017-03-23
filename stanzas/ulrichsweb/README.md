# Ulrichsweb
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/ulrichsweb.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/ulrichsweb.en.html) **

## Some of OCLC's notes for this stanza

Known issue with Ulrichsweb:

Due to security updates made in EZproxy 6.1 onwards, users may now get this message, "Connection refused by ulrichsweb.serialssolutions.com, please try again later."

This happens when attempting to use the HTTPS host as your starting point URL.

Resolution:

To work around this issue you can tell EZproxy to lower its SSL Security standards for outgoing requests by adding the following to config.txt, before the first LoginPortSSL directive:

Incoming connections to EZproxy are unaffected but outgoing requests will stop attempting to use TLSv1.2, which typically works around this issue. Please be aware, that adding this line will lower the security of your EZproxy server and will prevent you from accessing other vendors which mandate the use of TLSv1.2. This issue will persist until Ulrichsweb update their security.
