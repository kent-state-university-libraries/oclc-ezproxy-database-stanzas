# LoisLaw
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/lois_law.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/lois_law.en.html) **

## Some of OCLC's notes for this stanza

Lois Law requires the following configuration in the config.txt  file:

Title LoisLaw
 URL http://www.loislaw.com/pns/index.htp?content=/pns/aspen/asplibs.htp&
 DJ loislaw.com
 Find url: location.protocol+"//"+location.host+location.port
 Replace url: "http://^Awww.loislaw.com"
 Find ReturnURL=http://
 Replace ReturnURL=http://^A
 Find var EStoreHostHttp
 Replace var EStoreHostHttpProxied = "http://estore.loislaw.com"; var EStoreHostHttp = "http://^Aestore.loislaw.com"; //
 Find var EStoreHost
 Replace var EStoreHostProxied = "https://estore.loislaw.com"; var EStoreHost = "https://^Aestore.loislaw.com"; //
 Find var EcomHostHttp
 Replace var EcomHostHttpProxied = "http://ecom.loislaw.com"; var EcomHostHttp = "http://^Aecom.loislaw.com"; //
 Find var EcomHost
 Replace var EcomHostProxied = "https://ecom.loislaw.com"; var EcomHost = "https://^Aecom.loislaw.com"; //
 Find var targeturl = EStoreHostHttp
 Replace var targeturl = EStoreHostHttpProxied
 Find location.href = EStoreHost
 Replace location.href = EStoreHostProxied 
