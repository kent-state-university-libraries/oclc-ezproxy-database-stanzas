# Transparent Language
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/Transparent_Language](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/Transparent_Language) **

## Some of OCLC's notes for this stanza

In order to access Transparent Language Online for library customers, ensure that you construct your starting point URLs with your unique link as followed:

If your link was: https://ezproxy.mylib.org/login?url=https://library.transparent.com/[your library&rsquo;s nickname]/game/ng/#/login

Go to the URL Decoder/Encoder (meyerweb.com)&nbsp;and paste your link into the text field. Click encode and then copy the resulting text. In this example the text would become:

https%3A%2F%2Flibrary.transparent.com%2Fnickname%2Fgame%2Fng%2F%23%2Flogin

Create a link using that follows this pattern:

https://ezproxy.mylib.org/login?qurl=[your encoded link]

Using the example above it would be https://ezproxy.mylib.org/login?qurl=https%3A%2F%2Flibrary.transparent.com%2Fnickname%2Fgame%2Fng%2F%23%2Flogin

In order to access Transparent Language Online for education, customers can follow the same pattern except they will use the education.transparent.com subdomain. Example:

https://ezproxy.mylib.org/login?qurl=https%3A%2F%2Feducation.transparent.com%2Fnickname%2Fgame%2Fng%2F%23%2Flogin

A Hosted EZproxy Include File is available for this resource. Hosted EZproxy customers will receive automatic updates with OCLC&rsquo;s latest version of this stanza. Note: Hosted EZproxy customers in the Americas using self-service may reference the Include File by adding the following line to config.txt:

&nbsp;
