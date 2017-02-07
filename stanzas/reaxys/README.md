# Reaxys
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/reaxys.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/reaxys.en.html) **

## Some of OCLC's notes for this stanza

Effective January 28, 2017, Reaxys made changes to its new platform which will allow improved access via EZproxy. The new platform requires SSL Configuration and the following database stanza in config.txt:

Please note that this stanza was developed in a test environment and may require some adjustments as the migration continues.

The current (https://www.reaxys.com) and new (https://new.reaxys.com) Reaxys platforms will run in parallel until late this calendar year. We recommend keeping the previous stanza in place in config.txt until the migration is complete, and adding the new stanza above it.

When using both current and new Reaxys, the stanza for current Reaxys will need to be updated as below:

The line DJ www.reaxys.com formerly read DJ reaxys.com.

If you have registered your link resolver with Reaxys, the Replace statement in the new stanza will need to be modified as below:

If you have registered your link resolver with Reaxys, please use the following stanza for current Reaxys:

Replace "linkresolver.library.edu" with the URL of your link resolver.
