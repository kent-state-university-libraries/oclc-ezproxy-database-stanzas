# Factiva
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/factiva.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/factiva.en.html) **

## Some of OCLC's notes for this stanza

Title Factiva
 URL http://global.factiva.com
 Host https://global.factiva.com
 Host www.factiva.com
 DJ factiva.com
 DJ wsj.com
 DJ wsj.net
 DJ allthingsd.com
 DJ barrons.com
 DJ efinancialnews.com
 DJ marketwatch.com
 DJ smartmoney.com
 DJ wsjradio.com
 DJ dowjones.com
 DJ fins.com
 DJ wsjstudent.com
 DJ wsjwine.com
 Find targetsite=http://
 Replace targetsite=http://^A
 Find name="landingPage" value="http://
 Replace name="landingPage" value="http://^A
 Find name='LandingPage' value='http://
 Replace name='LandingPage' value='http://^A
 Find name="targetsite" value="http://
 Replace name="targetsite" value="http://^A

If you change your URL line to https, do NOT change the http in the Find and Replace lines. These Find and Replace lines should always contain http.

For Factiva to work, you must also follows the steps in SSL Configuration to enable the proxying of https pages as these are used during the Factiva login process.
