# OWASP juice shop solutions

Revisited to prepare for OSWE! https://github.com/juice-shop/juice-shop. 

## Installation


1.  Install [Docker](https://www.docker.com)
2.  Run `docker pull bkimminich/juice-shop`
3.  Run `docker run --rm -p 3000:3000 bkimminich/juice-shop`
4.  Browse to [http://localhost:3000](http://localhost:3000) (on macOS and Windows browse to [http://192.168.99.100:3000](http://192.168.99.100:3000) if you are using docker-machine instead of the native docker installation)


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
- [x] [Security Policy](../master/Level2/security-policy.md) 
- [x] [View Basket](../master/Level2/view-basket.md) - `Broken Access Control`
- [ ] [Visual Geo Stalking]()
- [x] [Weird Crypto](../master/Level2/wierd-crypto.md) - `Cryptographic Issues`

Old
- [x] [Classic Stored XSS](../master/Level2/classic-stored-xss.md) - `XSS`

### Level 3 Star challenge :star::star::star:

- [x] [Admin Registration](../master/Level3/admin-registration.md) - `Improper Input Validation`
- [x] [Bjoern's Favorite Pet](../master/Level3/bjoern-fav-pet.md) - `Broken Authentication`
- [x] [CAPTCHA Bypass](../master/Level3/captcha-by-pass.md) - `Broken Anti Automation`
- [x] [CSRF](../master/Level3/csrf.md) - `Broken Access Control`
- [x] [Database Schema](../master/Level3/database-schema.md) - `Injection`
- [x] [Deluxe Fraud](../master/Level3/deluxe-fraud.md) - `Improper Input Validation`
- [x] [Forged Feedback](../master/Level3/forged-feedback.md) - `Broken Access Control`
- [x] [Forged Review](../master/Level3/forged-feedback.md)) - `Broken Access Control`
- [ ] [GDPR Data Erasure](../master/Level3/.md)  - `Broken Authentication`
- [ ] [Login Amy](../master/Level3/.md)  - `Sensitive Data Exposure`
- [ ] [Login Bender](../master/Level3/.md) - `Injection`
- [ ] [Login Jim](../master/Level3/.md) - `Injection`
- [ ] [Manipulate Basket](../master/Level3/.md) - `Broken Access Control`
- [ ] [Payback Time](../master/Level3/.md) - `Improper Input Validation`
- [ ] [Privacy Policy Inspection](../master/Level3/.md) - `Security through Obscurity`
- [ ] [Product Tampering](../master/Level3/.md) - `Broken Access Control`
- [ ] [Reset Jim's Password](../master/Level3/.md) - `Broken Authentication`
- [ ] [Upload Size](../master/Level3/.md) - `Improper Input Validation`
- [x] [Upload Type](../master/Level3/upload-type.md) - `Improper Input Validation`

Old
- [x] [API-only XSS](../master/Level3/api-only-xss.md) - `XSS`
- [x] [Client-side XSS Protection](../master/Level3/client-side-xss.md) - `XSS`
- [x] [XXE Data Access](../master/Level3/xxe-data-access.md) - `XXE`


### Level 4 Star challenge :star::star::star: