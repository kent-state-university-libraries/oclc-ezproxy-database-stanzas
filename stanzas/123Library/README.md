# 123Library
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/EZproxy_database_stanzas/Database_stanzas_Numbers/123Library](https://help.oclc.org/Library_Management/EZproxy/EZproxy_database_stanzas/Database_stanzas_Numbers/123Library) **

## Some of OCLC's notes for this stanza

Important: Note the &ldquo;https&rdquo;.&nbsp; If you use &ldquo;http&rdquo;, you will encounter errors.

Note: There is no Host or Domain line. This is deliberate and intentional. 123Library uses a CDN (content delivery network) that requires other hosts on the 123library.org domain. These should not be proxied. The only URL you need to proxy for authentication purposes is the one given above.

You must ensure that your installation of EZproxy is set up for SSL, and for proxy by hostname. The relevant lines in your EZproxy config.txt will look something like this:

Finally, you will need to ensure that your DNS zone file includes records similar to the following, which are required in order to allow EZproxy to proxy by hostname. If you already use EZproxy for other services, this has probably already been done by your domain administrator:

In this example, 111.222.333.444 is the IP address of the server on which you have installed EZproxy.

A Hosted EZproxy Include File is available for this resource. Hosted EZproxy customers will receive automatic updates with OCLC&rsquo;s latest version of this stanza. Note: Hosted EZproxy customers in the Americas using self-service may reference the Include File by adding the following line to config.txt:

&nbsp;
