# Taylor & Francis eBooks
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/tandfebooks.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/tandfebooks.en.html) **

## Some of OCLC's notes for this stanza

Taylor & Francis eBooks requires SSL configuration and the following database stanza in config.txt :

If you are having trouble with the above stanza, try adding the following directive under "HTTPHeader authtoken":

If you are still having trouble, try adding the following the following directive under "DJ taylorfrancis.com":

The above directive is only necessary if you have another directive elsewhere in config.txt specifying that amazonaws.com should be proxied (e.g. "HJ amazonaws.com" or "DJ amazonaws.com"). Please note that NeverProxy directives are global in nature, so this may complicate debugging other stanzas.
