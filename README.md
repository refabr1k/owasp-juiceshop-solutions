# OWASP juice shop solutions

Revisited to prepare for OSWE! https://github.com/juice-shop/juice-shop. 

## Installation


1.  Install [Docker](https://www.docker.com)
2.  Run `docker pull bkimminich/juice-shop`
3.  Run `docker run --rm -p 3000:3000 bkimminich/juice-shop`
4.  Browse to [http://localhost:3000](http://localhost:3000) (on macOS and Windows browse to [http://192.168.99.100:3000](http://192.168.99.100:3000) if you are using docker-machine instead of the native docker installation)



```bash

# run unsafe mode to enable all challenge
docker run -d -e "NODE_ENV=unsafe" -p 3000:3000 bkimminich/juice-shop
```

## Solutions

### Level 1 Star challenge :star:
- [x] [Bonus Payload](../master/Level1/dom-xss.md) - `Improper Input Validation`
- [x] [Bully Chatbot](../master/Level1/bully-chatbot.md)
- [x] [Confidential Document](../master/Level1/confidential-doc.md) - `Sensitive Data Exposure`
- [x] [DOM XSS](../master/Level1/dom-xss.md) - `XSS`
- [x] [Error Handling](../master/Level1/error-handling.md) - `Security Misconfiguration`
- [x] [Exposed Metrics](Level1/exposed-metrics.md) - `Sensitive Data Exposure`
- [x] [Missing Encoding](../master/Level1/missing-encoding.md) - `Improper Input Validation`
- [x] [Outdated Whitelist](../master/Level1/outdated-whitelist.md) - `Unvalidated Redirects`
- [x] [Privacy Policy](../master/Level1/privacy-policy.md)
- [x] [Repetitive Registration](../master/Level1/repeat-register.md)  - `Improper Input Validation`
- [x] [Score Board](../master/Level1/score-board.md)
- [x] [Zero Stars](../master/Level1/zero-stars.md) - `Improper Input Validation`

Old
- [x] [Reflected XSS](../master/Level1/reflected-xss.md) - `XSS`

### Level 2 Star challenge :star::star:

- [x] [Admin Section](../master/Level2/admin-section.md) - `Broken Access Control`
- [x] [Deprecated Interface](../master/Level2/deprecated-interface.md) - `Security Misconfiguration`
- [x] [Five-Star Feedback](../master/Level2/five-star-feedback.md) - `Broken Access Control`
- [x] [Login Admin](../master/Level2/login-admin.md) - `Injection`
- [ ] [Login MC SafeSearch]()
- [ ] [Meta Geo Stalking]()
- [x] [Password Strength](../master/Level2/password-strength.md) - `Broken Authentication`
- [x] [Reflected XSS](../master/Level2/reflected-xss.md) - `XSS`
- [x] [Security Policy](../master/Level2/security-policy.md) 
- [x] [View Basket](../master/Level2/view-basket.md) - `Broken Access Control`
- [ ] [Visual Geo Stalking]()
- [x] [Weird Crypto](../master/Level2/wierd-crypto.md) - `Cryptographic Issues`

Old


### Level 3 Star challenge :star::star::star:
- [x] [API-only XSS](../master/Level3/api-only-xss.md) - `XSS`
- [x] [Admin Registration](../master/Level3/admin-registration.md) - `Improper Input Validation`
- [x] [Bjoern's Favorite Pet](../master/Level3/bjoern-fav-pet.md) - `Broken Authentication`
- [x] [CAPTCHA Bypass](../master/Level3/captcha-by-pass.md) - `Broken Anti Automation`
- [x] [CSRF](../master/Level3/csrf.md) - `Broken Access Control`
- [x] [Client-side XSS Protection](../master/Level3/client-side-xss.md) - `XSS`
- [x] [Database Schema](../master/Level3/database-schema.md) - `Injection`
- [x] [Deluxe Fraud](../master/Level3/deluxe-fraud.md) - `Improper Input Validation`
- [x] [Forged Feedback](../master/Level3/forged-feedback.md) - `Broken Access Control`
- [x] [Forged Review](../master/Level3/forged-feedback.md) - `Broken Access Control`
- [ ] [GDPR Data Erasure](../master/Level3/.md)  - `Broken Authentication`
- [x] [Login Amy](../master/Level3/login-user-account.md)  - `Sensitive Data Exposure` 
- [x] [Login Bender](../master/Level3/login-user-account.md) - `Injection`
- [x] [Login Jim](../master/Level3/login-user-account.md) - `Injection`
- [x] [Manipulate Basket](../master/Level3/add-to-other-basket.md) - `Broken Access Control`
- [x] [Payback Time](../master/Level3/payback-time.md) - `Improper Input Validation`
- [ ] [Privacy Policy Inspection](../master/Level3/.md) - `Security through Obscurity`
- [x] [Product Tampering](../master/Level3/product-tampering.md) - `Broken Access Control`
- [ ] [Reset Jim's Password](../master/Level3/.md) - `Broken Authentication`
- [ ] [Upload Size](../master/Level3/.md) - `Improper Input Validation`
- [x] [Upload Type](../master/Level3/upload-type.md) - `Improper Input Validation`
- [x] [XXE Data Access](../master/Level3/xxe-data-access.md) - `XXE`


### Level 4 Star challenge :star::star::star::star:
- [ ] [Access Log](.md) - `Sensitive Data Exposure`
- [ ] [Allowlist Bypass](.md) - `Unvalidated Redirects`
- [x] [CSP Bypass](../master/Level4/csp-xss.md) - `XSS`
- [ ] [Christmas Special](.md) - `Injection`
- [ ] [Easter Egg](.md) - `Broken Access Control`
- [ ] [Ephemeral Accountant](.md) - `Injection`
- [ ] [Expired Coupon](.md) - `Improper Input Validation`
- [ ] [Forgotten Sales Backup](.md) - `Sensitive Data Exposure`
- [ ] [GPDR Data Theft](.md) - `Senstive Data Exposure`
- [x] [HTTP-Header XSS](../master/Level4/xss-header.md) - `XSS`
- [ ] [Leaked Unsafe Product](.md) - `Sensitive Data Exposure`
- [ ] [Legacy Typosquatting](.md) - `Vulnerable Components`
- [ ] [Login Bjoern](.md) - `Broken Authentication`
- [ ] [Misplaced Signature File](.md) - `Sensitive Data Exposure`
- [ ] [Nested Easter Egg](.md) - `Cryptographic Issues`
- [x] [NoSQL Dos](../master/Level4/no-sql-sleep.md) - `Injection`
- [ ] [NoSQL Manipulation](.md) - `Injection`
- [ ] [Poison Null Byte](.md) - `Improper Input Validation`
- [ ] [Reset Bender's Password](.md) - `Broken Authentication`
- [ ] [Reset Uvogin's Password](.md) - `Sensitive Data Exposure`
- [x] [Server-side XSS Protection](../master/Level4/server-side-xss.md) - `XSS`
- [ ] [Steganography](.md) - `Security Through Obscurity`
- [ ] [User Credentials](.md) - `Injection`
- [ ] [Vulnerable Library](.md) - `Vulnerable Components`