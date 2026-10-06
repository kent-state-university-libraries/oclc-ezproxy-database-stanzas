# Kortext
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/EZproxy_database_stanzas/Database_stanzas_K/Kortext](https://help.oclc.org/Library_Management/EZproxy/EZproxy_database_stanzas/Database_stanzas_K/Kortext) **

## Some of OCLC's notes for this stanza

Kortext supports two EZproxy authentication methods: IP authentication and Single Sign-On (SSO). Use the stanza that matches the authentication method configured by Kortext. Kortext provides the URL to proxy, including the providerId, loginSource, and returnUrl parameters. Contact Kortext for the URL configured for your institution.

 Caution: Do not proxy app.kortext.com. EZproxy proxies the initial request to read.kortext.com; after authentication, Kortext redirects the user to app.kortext.com to access the resource directly.

 Note: Contact Kortext to obtain the URL to use in this stanza.

(for example, https://read.kortext.com/api/identity/v1/ezproxy/callback?providerId=XXXX&loginSource=&returnUrl=)

The URL provided by Kortext includes the providerId and a returnUrl that points to the app.kortext.com URL for the item. EZproxy proxies the initial request to Kortext; after authorization, the user is redirected directly to the app.kortext.com URL.

Replace the URL with the URL provided by Kortext.

 

 
