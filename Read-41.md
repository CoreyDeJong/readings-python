## Web Application Security
- The majority of web application attacks occur through cross-site scripting (XSS) and SQL injection attacks which typically are made possible by flawed coding and failure to sanitize application inputs and outputs.
- Secure web application development should be enhanced by applying security checkpoints and techniques at early stages of development as well as throughout the software development lifecycle.
- Special emphasis should be applied to the coding phase of development. Security mechanisms that should be used include, threat modeling, risk analysis, static analysis, digital signature, among others
- While security is fundamentally based on people and processes, there are a number of technical solutions to consider when designing, building and testing secure web applications. At a high level, these solutions include:

    - Black box testing tools such as Web application security scanners, vulnerability scanners and penetration testing software
    - White box testing tools such as static source code analyzers
    - Fuzzing tools used for input testing
    - Web application security scanner (vulnerability scanner)
    - Web application firewalls (WAF), used to provide firewall-type protection at the web application layer
    - Password cracking tools for testing password strength and implementation


## Django Security
- XSS attacks allow a user to inject client side scripts into the browsers of other users. 
- This is usually achieved by storing the malicious scripts in the database where it will be retrieved and displayed to other users, or by getting users to click a link which will cause the attacker’s JavaScript to be executed by the user’s browser.
- However, XSS attacks can originate from any untrusted source of data, such as cookies or Web services, whenever the data is not sufficiently sanitized before including in a page
- Cross site request forgery (CSRF) attacks allow a malicious user to execute actions using the credentials of another user without that user’s knowledge or consent.
- SQL injection is a type of attack where a malicious user is able to execute arbitrary SQL code on a database. This can result in records being deleted or data leakage.
- Clickjacking is a type of attack where a malicious site wraps another site in a frame. This attack can result in an unsuspecting user being tricked into performing unintended actions on the target site.