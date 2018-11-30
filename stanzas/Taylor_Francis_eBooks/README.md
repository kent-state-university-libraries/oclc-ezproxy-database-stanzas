# Taylor & Francis Ebooks
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/Taylor_Francis_eBooks](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/Taylor_Francis_eBooks) **

## Some of OCLC's notes for this stanza

If you are having trouble with the above stanza, try adding the following directive under &quot;HTTPHeader authtoken&quot;:

If you are still having trouble, try adding the following the following directive under &quot;DJ taylorfrancis.com&quot;:

The above directive is only necessary if you have another directive elsewhere in config.txt specifying that amazonaws.com should be proxied (e.g. &quot;HJ amazonaws.com&quot; or &quot;DJ amazonaws.com&quot;). Please note that NeverProxy directives are global in nature, so this may complicate debugging other stanzas.
