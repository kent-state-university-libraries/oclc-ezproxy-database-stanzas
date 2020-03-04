# E-Libro
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/E-Libro](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/E-Libro) **

## Some of OCLC's notes for this stanza

E-Libro has two options for remote access: IP Authentication using a stanza or Single sign-on (SSO). Please confirm which method you are using with E-Libro.

IP Authentication: Please add the following stanza to your EZproxy config.txt file to proxy E-LIbro.

Single sign-on (SSO): To establish single sign-on support between EZproxy and E-Libro, add the following line to config.txt:

Values for {secret} and {url} are provided by E-Libro.

Example:

In addition, to ensure access to your institution&rsquo;s subscribed resources, you must construct your E-Libro URLs using your institution&rsquo;s unique context number. See the following example:&nbsp;

Replace ##### with the context number provided to you by E-Libro.

&nbsp;
