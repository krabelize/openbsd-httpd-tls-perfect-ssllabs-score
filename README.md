# OpenBSD httpd TLS config with Let's Encrypt
OpenBSD httpd configuration for perfect TLS SSL Labs score A+ with Let's Encrypt

![ssllabs-perfect-score](https://cryptsus.com/blog/ssl-labs-a-plus.jpg)


**Server Key and Certificate #1**

Subject cryptsus.com

Fingerprint SHA256: fingerprint

Pin SHA256: pin

Common names cryptsus.com

Alternative names	cryptsus.com www.cryptsus.com

Serial Number	03f4b8b6ae311dc8bc877674695719379e07

Valid from	Wed, 20 Jan 2021 22:01:02 UTC

Valid until	Tue, 20 Apr 2021 22:01:02 UTC (expires in 30 days, 9 hours)

Key	RSA 4096 bits (e 65537)

Weak key (Debian)	No

Issuer	R3

AIA: http://r3.i.lencr.org/

Signature algorithm	SHA256withRSA

Extended Validation	No

Certificate Transparency	Yes (certificate)

OCSP Must Staple	No

Revocation information	OCSP http://r3.o.lencr.org

Revocation status	Good (not revoked)

DNS CAA	Yes issue: letsencrypt.org flags:0

Trusted	Yes Mozilla  Apple  Android  Java  Windows 

**Additional Certificates (if supplied)**

Subject	R3 Fingerprint SHA256: 730c1bdcd85f57ce5dc0bba733e5f1ba5a925b2a771d640a26f7a454224dad3b Pin SHA256: jQJTbIh0grw0/1TkHSumWb+Fs0Ggogr621gT3PvPKG0=

Valid until	Wed, 29 Sep 2021 19:21:40 UTC (expires in 6 months and 8 days)

Key	RSA 2048 bits (e 65537)

Issuer	DST Root CA X3

Signature algorithm	SHA256withRSA

**Protocols**

TLS 1.3	Yes
TLS 1.2	Yes
TLS 1.1	No
TLS 1.0	No
SSL 3	No
SSL 2	No

**Cipher Suites**
 
# TLS 1.3 (suites in server-preferred order)
```
TLS_AES_256_GCM_SHA384 (0x1302)   ECDH secp384r1 (eq. 7680 bits RSA)   FS	256
TLS_CHACHA20_POLY1305_SHA256 (0x1303)   ECDH secp384r1 (eq. 7680 bits RSA)   FS	256
TLS_AES_128_GCM_SHA256 (0x1301)   ECDH secp384r1 (eq. 7680 bits RSA)   FS	128	
```

# TLS 1.2 (suites in server-preferred order)
```
TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384 (0xc030)   ECDH secp384r1 (eq. 7680 bits RSA)   FS	256	
TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305_SHA256 (0xcca8)   ECDH secp384r1 (eq. 7680 bits RSA)   FS	256
TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256 (0xc02f)   ECDH secp384r1 (eq. 7680 bits RSA)   FS	128
```

**Handshake Simulation**

```
Android 4.4.2 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Android 5.0.0 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256   ECDH secp384r1  FS
Android 6.0 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256   ECDH secp384r1  FS
Android 7.0 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Android 8.0 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Android 8.1 - TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
Android 9.0 - TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
BingPreview Jan 2015 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Chrome 49 / XP SP3 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305_SHA256   ECDH secp384r1  FS
Chrome 69 / Win 7  R - TLS 1.2	TLS_AES_256_GCM_SHA384  FS
Chrome 70 / Win 10 - TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
Chrome 80 / Win 10  R -	TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
Firefox 31.3.0 ESR / Win 7 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256   ECDH secp384r1  FS
Firefox 47 / Win 7  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305_SHA256   ECDH secp384r1  FS
Firefox 49 / XP SP3 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Firefox 62 / Win 7  R - TLS 1.2	TLS_AES_256_GCM_SHA384  FS
Firefox 73 / Win 10  R -	TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
Googlebot Feb 2018 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
IE 11 / Win 7  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384   ECDH secp384r1  FS
IE 11 / Win 8.1  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384   ECDH secp384r1  FS
IE 11 / Win Phone 8.1  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA   ECDH secp384r1  FS
IE 11 / Win Phone 8.1 Update  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384   ECDH secp384r1  FS
IE 11 / Win 10  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Edge 15 / Win 10  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Edge 16 / Win 10  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Edge 18 / Win 10  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Edge 13 / Win Phone 10  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Java 8u161 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Java 11.0.3 - TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
Java 12.0.1 - TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
OpenSSL 1.0.1l  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
OpenSSL 1.0.2s  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
OpenSSL 1.1.0k  R - TLS 1.2	TLS_AES_256_GCM_SHA384  FS
OpenSSL 1.1.1c  R - TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
Safari 6 / iOS 6.0.1 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384   ECDH secp384r1  FS
Safari 7 / iOS 7.1  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384   ECDH secp384r1  FS
Safari 7 / OS X 10.9  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384   ECDH secp384r1  FS
Safari 8 / iOS 8.4  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384   ECDH secp384r1  FS
Safari 8 / OS X 10.10  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384   ECDH secp384r1  FS
Safari 9 / iOS 9  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Safari 9 / OS X 10.11  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Safari 10 / iOS 10  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Safari 10 / OS X 10.12  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Safari 12.1.2 / MacOS 10.14.6 Beta  R - TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
Safari 12.1.1 / iOS 12.3.1  R - TLS 1.3	TLS_AES_256_GCM_SHA384   ECDH secp384r1  FS
Apple ATS 9 / iOS 9  R RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
Yahoo Slurp Jan 2015 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
YandexBot Jan 2015 RSA 4096 (SHA256) TLS 1.2	TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384   ECDH secp384r1  FS
```

**Protocol Details**

DROWN	No, server keys and hostname not seen elsewhere with SSLv2

Secure Renegotiation	Supported

Secure Client-Initiated Renegotiation	No

Insecure Client-Initiated Renegotiation	No

BEAST attack	Mitigated server-side 

POODLE (SSLv3)	No, SSL 3 not supported

POODLE (TLS)	No

Zombie POODLE	No TLS 1.2 : 0xc014

GOLDENDOODLE	No TLS 1.2 : 0xc014

OpenSSL 0-Length	No TLS 1.2 : 0xc014

Sleeping POODLE	No TLS 1.2 : 0xc014

Downgrade attack prevention	Yes, TLS_FALLBACK_SCSV supported

SSL/TLS compression	No

RC4	No

Heartbeat (extension)	No

Heartbleed (vulnerability)

Ticketbleed (vulnerability)

OpenSSL CCS vuln. (CVE-2014-0224)	No

OpenSSL Padding Oracle vuln. (CVE-2016-2107)

ROBOT (vulnerability)	No (more info)

Forward Secrecy	Yes (with most browsers) ROBUST

ALPN	No

NPN	No

Session resumption (caching)	No (IDs empty)

Session resumption (tickets)	Yes

OCSP stapling	Yes

Strict Transport Security (HSTS)	Yes

max-age=31536000; includeSubDomains; preload

HSTS Preloading	Chrome  Edge  Firefox  IE   

Public Key Pinning (HPKP)	No

Public Key Pinning Report-Only	No

Public Key Pinning (Static)	No

Long handshake intolerance	No

TLS extension intolerance	No

TLS version intolerance	No

Incorrect SNI alerts	No

Uses common DH primes	No, DHE suites not supported

DH public server param (Ys) reuse	No, DHE suites not supported

ECDH public server param reuse	No

Supported Named Groups	secp384r1

SSL 2 handshake compatibility	No

0-RTT enabled	No

**Miscellaneous**

Test date	Sun, 21 Mar 2021 12:41:30 UTC

Test duration	81.946 seconds

HTTP status code	200

HTTP server signature	OpenBSD httpd

Server hostname	cryptsus.com
