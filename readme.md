### Thoughts
```
Minor quibble:
   WHY CAN'T I USE TLS/SSL TO DELIVER THE JAVASCRIPT
   CRYPTO CODE?

   You can. It's harder than it sounds, but you safely
   transmit Javascript crypto to a browser using SSL. The
   problem is, having established a secure channel with SSL,
   you no longer need Javascript cryptography; you have "real"
   cryptography. Meanwhile, the Javascript crypto code is still
   imperiled by other browser problems
```
```
I have only heard of one application of JS crypto that made sense,
but it wasn't from a security perspective. A web firm processes credit card numbers. For cost reasons,
they wanted to avoid PCI audits of their webservers, but PCI required any server that handled
plaintext credit card numbers to be audited. So, their webservers send a JS crypto app to the
browser client to encrypt the credit card number with an RSA public key. The corresponding private key
is accessible only to the backend database. So based on the
wording of PCI, only the database server requires an audit.
```

### Threads
Thread from 2014: https://news.ycombinator.com/item?id=7903720
2013: https://news.ycombinator.com/item?id=5123165
Discussed at the time: https://news.ycombinator.com/item?id=2935220
https://rdist.root.org/2010/11/29/final-post-on-javascript-crypto/

### Labs
http://hub.docker.com/r/bhattsameer/jsdebugginglab

### Videos
#### Martin Boßlet: Javascript Crypto. Ugly duckling with good reason? -- JSConf EU 2013
https://youtu.be/NjMOSg5Pe44?si=nkzkMN21g5djyffw
