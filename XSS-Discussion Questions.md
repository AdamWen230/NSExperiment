#### Q1: What are the main differences of CSRF and XSS attacks? They both have “cross site” in their names.

A1：The main differences of CSRF and XSS attack is where the malicious code is executed. In CSRF attack, the attacker make the victim click the url he sends, and the forged HTTP request was send by the malicious website's page, not the original page. But in the XSS attack, the malicious code was injected into the victim's page and database, it is executed at the website's  own page. They both have cross site in their names is because in CSRF attack, the malicious code is executed on another site while in XSS attack the malicious code was first created and stored in another site and then injected into the victim's page.



#### Q2: Can we use the countermeasures against CSRF attacks to defend against XSS attacks, including the secret token and same-site cookie approaches?



A2: Since the malicious code is stored in the victim's page, the malicious code can easily get the secret token as well as the same-site cookie to forge the correct HTTP request, so that the countermeasures against CSRF attacks can not defend the XSS attacks. 

