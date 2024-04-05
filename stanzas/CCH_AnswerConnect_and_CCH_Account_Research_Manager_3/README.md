# CCH AnswerConnect and CCH Account Research Manager 3.0
** This stanza needs manual review at [https://help.oclc.org/Library_Management/EZproxy/EZproxy_database_stanzas/Database_stanzas_C/CCH_AnswerConnect_and_CCH_Account_Research_Manager_3.0](https://help.oclc.org/Library_Management/EZproxy/EZproxy_database_stanzas/Database_stanzas_C/CCH_AnswerConnect_and_CCH_Account_Research_Manager_3.0) **

## Some of OCLC's notes for this stanza

&nbsp; Note:&nbsp;If your config.txt file contains stanzas for both CCH AnswerConnect and CCH Account Research Manager 3.0 and Vitallaw Premium, make sure that the CCH AnswerConnect and CCH Account Research Manager 3.0 is above the Wiley Online Library stanza. This will ensure that processing of the CCH AnswerConnect and CCH Account Research Manager 3.0 stanza includes all processing directives in that stanza but will not interfere with the processing of the Vitallaw Premium stanza.

&nbsp;

&nbsp; Note: To access CCH Answerconnect you must use the following starting point URL:

https://your.ezproxy.server.address/login?url=https://www.answerconnect.cch.com

Replace your.ezproxy.server.address with the hostname of your EZproxy server:

&nbsp;

&nbsp; Note: To access&nbsp;CCH Account Research Manager 3.0 you must use the following starting point URL:

https://your.ezproxy.server.address/login?url=https://answerconnect.cch.com/api/2.0/protected/navigation/openHomePage?tab=accounting

Replace&nbsp; your.ezproxy.server.address with the hostname of your EZproxy server

&nbsp;

A Hosted EZproxy Include File is available for this resource. Hosted EZproxy customers will receive automatic updates with OCLC&rsquo;s latest version of this stanza. Note: Hosted EZproxy customers in the Americas using self-service may reference the Include File by adding the following line to config.txt:

&nbsp;
