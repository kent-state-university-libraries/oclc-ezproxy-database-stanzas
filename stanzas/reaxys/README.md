# Reaxys
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/reaxys.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/reaxys.en.html) **

## Some of OCLC's notes for this stanza

Effective January 28, 2017, Reaxys 2 was changed to allow improved access via EZproxy. Reaxys 2 requires EZproxy 6.2.2, SSL Configuration and the following database stanza in config.txt:

Title Reaxys 2
 URL https://www.reaxys.com
 HJ https://www.reaxys.com
 HJ https://sc.elsevier.com
 HJ sc.elsevier.com
 DJ www.reaxys.com
 DJ elsevier.com
 # DOI system provides linking to Springer, Wiley, and others
 DJ dx.doi.org
 Find .replace("OLD_EXTERNAL_URL","NEW_EXTERNAL_URL")
 Replace .replace("linksolver.ovid.com","^plinksolver.ovid.com^").replace("sc.elsevier.com","^psc.elsevier.com^").replace("lls.reaxys.com","^slls.reaxys.com^")

Please note that this stanza was developed in a test environment and may require some adjustments as the migration continues.

Reaxys 1 (still available under https://rx1.reaxys.com) and Reaxys 2 (available through https://www.reaxys.com) will run in parallel until the end of May, 2018. We recommend keeping the previous stanza in place in config.txt until the migration is complete, and adding the new stanza above it.

When using both Reaxys 1 and Reaxys 2, the stanza for Reaxys 1 will need to be updated as below:

Title Reaxys 1
 URL https://rx1.reaxys.com
 DJ rx1.reaxys.com
 HJ https://rx1.reaxys.com
 HJ sc.elsevier.com
 Find window.open(response)
 Replace window.open(response.replace('linksolver.ovid.com', '^plinksolver.ovid.com^').replace('sc.elsevier.com', '^psc.elsevier.com^').replace('lls.reaxys.com', '^slls.reaxys.com^'))

The line "DJ https://rx1.reaxys.com" formerly read "DJ reaxys.com".

If you have registered your link resolver with Reaxys, the Replace statement in the new stanza for Reaxys 2 will need to be modified as below:

Replace .replace("linksolver.ovid.com","^plinksolver.ovid.com^").replace("sc.elsevier.com","^psc.elsevier.com^").replace("lls.reaxys.com","^slls.reaxys.com^").replace("linkresolver.library.edu","^plinkresolver.library.edu^")

If you have registered your link resolver with Reaxys, please use the following stanza for Reaxys 1:

Title Reaxys
 MimeFilter text/json-comment-filtered .* html
 URL https://rx1.reaxys.com
 DJ rx1.reaxys.com
 HJ https://rx1.reaxys.com
 HJ sc.elsevier.com
 Find window.open(response)
 Replace window.open(response.replace('linksolver.ovid.com', '^plinksolver.ovid.com^').replace('sc.elsevier.com', '^psc.elsevier.com^').replace('lls.reaxys.com', '^slls.reaxys.com^'))
 Find linkresolver.library.edu
 Replace ^plinkresolver.library.edu^

Replace "linkresolver.library.edu" with the URL of your link resolver.
