# Books24x7
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/Books24x7](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/Books24x7) **

## Some of OCLC's notes for this stanza

In starting point URLs for Books24x7, the ^B will be replaced by a encrypted packet of information that contains the current date and time, the IP address of the remote user, and an encrypted version of the user's username.

ABC123 is replaced by the site identifier issued to you by Books24x7.

SomethingYouPickAndDontTellAnyone is a random string that you pick that is used to encrypt the username of the person accessing EZproxy before sending it to Books24x7

YouGetThisFromBooks24x7 is used to encrypt a combination of the IP address making the request and the encrypted username formed with TokenKey, or just the IP address if someone is accessing from within an ExcludeIP range.

This process does not disclose the identity of the EZproxy user to Books24x7, but instead sends an encrypted string that allows Books24x7 to know that the same user is accessing, but nothing about the original username. If necessary, Books24x7 can provide your library with this encrypted string, then you can cross-reference it to the original user using the administration page option for Decode Token Key.

&nbsp;
