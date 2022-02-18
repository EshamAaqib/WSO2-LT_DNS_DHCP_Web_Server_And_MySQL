# WSO2_DNS_DHCP_Web_Server_And_MySQL_Assignment


## URL - lt-2021-047.ml or www.lt-2021-047.ml 

## URL (Configuration Files and Public Key; I used gitfront.io to share the private GitHub Repository) - https://gitfront.io/r/eshamaaqib/2a40ab4bd5f5beb0cb728c4332b67d21e73e73ab/WSO2-DNS-DHCP-Web-Server-And-MySQL-Assignment/

## Screenshot of DNS Records 

### I had few issues with Freenom DNS and the changes didn't propagate after even waiting for hours, even re-registering didn't fix the issue so as we had access to GCP I switched to Google DNS and it worked well.

###### Screenshot of the Nameserver
![Nameservers](https://user-images.githubusercontent.com/75664650/128033123-4c31f807-a8f6-4081-8b2d-8f225115f818.png)

###### Screenshot of DNS Records
![DNS_Records](https://user-images.githubusercontent.com/75664650/128033178-2a579437-76b6-4595-af6f-7bf815f21af2.png)


## Mail Service

### I went ahead moved from ImprovMX to Yandex Mail as Yandex also has a free plan and had more features. Additionally it was extremely useful when doing email security hardening part. (No credit cards were used as it is completely free)

![Yandex Plan](https://user-images.githubusercontent.com/75664650/128034372-d3372481-b7dc-47a3-9392-186cf31b259a.png)

![Yandex Domain](https://user-images.githubusercontent.com/75664650/128034396-80ebf847-4fa8-4b06-a65c-a0da2f790ce6.png)

![WSO2_Reply](https://user-images.githubusercontent.com/75664650/128034800-e9de875d-8982-4653-ae3d-4f4c6d5b57d2.png)

## The Public key used to enable HTTPS on the website

```
-----BEGIN PUBLIC KEY-----
MIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEA2Wb4LhWsLxAZoEHcD6ue
iaY/EBXwb+fpWAjW6P4il+CVIjjrOMZurxfomdw7zJFsSG61PhUTdhEWnbLeLQxR
tn2Cpr0FolpNEQlBGa4f+VPO1/xwX3mVK9p7suM4Z18QQcvjb82IzGAzisweO8LW
oDSOjm0OwF/mwI1E78IFi38jB3k/d8axwxvhpzl+BuVNjkFTwq4MeYoKmtWeQD3v
YQ7+Cqk5vLaja0SDLVUiEKDnzsQGblCkEPi7IE87hqgqANKKg2hUEmfOj/xwd7r9
FeTYb+Z0mLDeOTCMYUrOZb1JgoU/D41KgcyhqlyLPFE88OyIPjsz8zbeAz+72LZD
HoyxPnfnHsLZQ73rzwgGSl7kkeZxkmGPmi0WvMYCpOnAwINo9HCycy31K47tbgAp
oOXOL0T5wstHPq+iPyPAtG0VYGBTfmqlslaQshSdPzurJvz2+1o9UQZJ4Y3ZBQhu
wIjKAVDiUcL1dRHOktOVE4YLjDgdOxZSp9pSudKzAwpSVDRDiJXSirsSt+dyF6jH
DPYViTokFetR38MqE7n+hqlWFdhI6tP2zz4A6OvQudKs5Sh1hM2na0Nd03hg2G6b
CxHywgrWfsLyjii2WufGIEz5Do1RoJ/BEBAJi/eH0bUnXV77zhku+p3n775ZXP+R
0e1YRYGVYygujDAnEB+6AWsCAwEAAQ==
-----END PUBLIC KEY-----
```

## Nginx Host Config File and SSL Configuration file is available in the Nginx Host Config Folder


## Nginx Security Hardening 

### 1) Using a 4096 Bit RSA SSL Certificate
### 2) Disabled weak SSL/TLS protocols
### 3) Disabled weak cipher suites and added stronger ones
### 4) Secure Diffie-Hellman for TLS
### 5) Enabled HTTP Strict Transport Security
### 6) Enabled DNSSEC
### 7) Disabled unwanted HTTP methods
### 8) Disabled direct IP access
### 9) Clickjacking Attack prevention
### 10) X-XSS Protection
### 11) Excluded Server Headers
### 12) Prevented Buffer Overflow
### 13) DNS Certification Authority Authorization (CAA) Policy


### SSL Labs Test Screenshot
![SSLLabs](https://user-images.githubusercontent.com/75664650/128040080-8e27acab-3cd1-4b62-8803-4d0d6c4a40b4.png)

## Email Security Hardening 

### 1) Added SPF Records
### 2) Added DMARC Policy
### 3) Added DKIM Records
### 4) Encrypted Outgoing Mail with S/MIME Certificate (Free certificate issued by Actalis ; https://extrassl.actalis.it/portal/uapub/freemail?lang=en)

### As a result of using S/MIME the receiver would see the email address "admin@lt-2021-047.ml" as a verified email address. Screenshot below.

![MIME](https://user-images.githubusercontent.com/75664650/128041233-d111505e-da9e-4ac5-914b-5ac6573dd2f8.png)



