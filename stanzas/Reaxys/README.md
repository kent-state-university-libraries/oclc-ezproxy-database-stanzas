# Reaxys
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/Reaxys](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas/Reaxys) **

## Some of OCLC's notes for this stanza

Effective January 28, 2017, Reaxys made changes to its new platform which will allow improved access via EZproxy. The new platform requires EZproxy 6.2.2

Please note that this stanza was developed in a test environment and may require some adjustments as the migration continues.

Reaxys 1 (still available under https://rx1.reaxys.com) and Reaxys 2 (available through https://www.reaxys.com) will run in parallel until&nbsp;the end of May, 2018. We recommend keeping the previous stanza in place in config.txt until the migration is complete, and adding the new stanza above it.

When using both Reaxys 1 and Reaxys 2, the stanza for Reaxys 1 will need to be updated as below:

The line DJ https://rx1.reaxys.com formerly read DJ reaxys.com.

If you have registered your link resolver with Reaxys, the Replace statement in the new stanza will need to be modified as below:

If you have registered your link resolver with Reaxys, please use the following stanza for Reaxys 1:

Replace linkresolver.library.edu with the URL of your link resolver.

A Hosted EZproxy Include File is available for this resource. Hosted EZproxy customers will receive automatic updates with OCLC&rsquo;s latest version of this stanza by adding the following line to config.txt:
