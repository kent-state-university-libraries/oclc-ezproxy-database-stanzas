# 123Library
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/123library.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/123library.en.html) **

## Some of OCLC's notes for this stanza

123Library requires the following configuration in config.txt :

Please note the “https”. If you use “http”, you will encounter errors.

Please note also that there is no Host or Domain line. This is deliberate and intentional. 123Library uses a CDN (content delivery network) that requires other hosts on the 123library.org domain. These should not be proxied. The only URL you need to proxy for authentication purposes is the one given above.

You will also need to ensure that your installation of EZproxy is set up for SSL, and for proxy by hostname. The relevant lines in your EZproxy config.txt will look something like this:

Finally, you will need to ensure that your DNS zone file includes records similar to the following, which are required in order to allow EZproxy to proxy by hostname. If you already use EZproxy for other services, this has probably already been done by your domain administrator:

In this example, 111.222.333.444 is the IP address of the server on which you have installed EZproxy.
