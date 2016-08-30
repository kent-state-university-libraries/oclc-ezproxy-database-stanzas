# SRDS
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/srds.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/srds.en.html) **

## Some of OCLC's notes for this stanza

HTTPHeader X-Requested-With
 Title SRDS
 URL http://next.srds.com
 DJ srds.com

If using EZproxy v6.1 or later, you must include the following SSL command prior to any LoginPortSSL directive to disable the use of TLSv1.2 in outgoing connections from EZproxy to allow EZproxy to communicate with https://www.srds.com successfully: 

SSLOpenSSLConfCmd -Cert=-1 Protocol -TLSv1.2

Note: This stanza works best when it is the first stanza in the database stanza list.
