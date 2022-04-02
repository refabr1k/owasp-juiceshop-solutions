# OWASP juice shop solutions

Revisited to prepare for OSWE! https://github.com/juice-shop/juice-shop. 

## Installation


1.  Install [Docker](https://www.docker.com)
2.  Run `docker pull bkimminich/juice-shop`
3.  Run `docker run --rm -p 3000:3000 bkimminich/juice-shop`
4.  Browse to [http://localhost:3000](http://localhost:3000) (on macOS and Windows browse to [http://192.168.99.100:3000](http://192.168.99.100:3000) if you are using docker-machine instead of the native docker installation)


## Solutions

### Level 1 Star challenge
- [ ] [Bonus Payload]()
- [ ] [Bully Chatbot]()
- [x] [Confidential Document](../master/Level1/confidential-doc.md)
- [x] [DOM XSS](../master/Level1/dom-xss.md)
- [x] [Error Handling](../master/Level1/error-handling.md)
- [x] [Exposed Metrics](Level1/exposed-metrics.md))
- [x] [Missing Encoding](../master/Level1/missing-encoding.md)
- [x] [Outdated Whitelist](../master/Level1/outdated-whitelist.md)
- [x] [Privacy Policy](../master/Level1/privacy-policy.md)
- [x] [Repetitive Registration](../master/Level1/repeat-register.md)
- [x] [Score Board](../master/Level1/score-board.md)
- [x] [Zero Stars](../master/Level1/zero-stars.md)

Old
- [x] [Reflected XSS](../master/Level1/reflected-xss.md)

### Level 2 Star challenge

- [x] [Admin Section](../master/Level2/admin-section.md)
- [x] [Classic Stored XSS](../master/Level2/classic-stored-xss.md)
- [x] [Deprecated Interface](../master/Level2/deprecated-interface.md)
- [x] [Five-Star Feedback](../master/Level2/five-star-feedback.md)
- [x] [Login Admin](../master/Level2/login-admin.md)
- [ ] [Login MC SafeSearch]()
- [x] [Password Strength](../master/Level2/password-strength.md)
- [x] [Security Policy](../master/Level2/security-policy.md)
- [x] [View Basket](../master/Level2/view-basket.md)
- [x] [Weird Crypto](../master/Level2/wierd-crypto.md)

### Level 3 Star challenge

- [x] [API-only XSS](../master/Level3/api-only-xss.md)
- [x] [Admin Registration](../master/Level3/admin-registration.md)
- [x] [Bjoern's Favorite Pet](../master/Level3/bjoern-fav-pet.md)
- [x] [CAPTCHA Bypass](../master/Level3/captcha-by-pass.md)
- [x] [Client-side XSS Protection](../master/Level3/client-side-xss.md)
- [x] [Database Schema](../master/Level3/database-schema.md)
- [ ] [Forged Feedback](../master/Level3/.md)
- [ ] [Forged Review](../master/Level3/.md)
- [ ] [GDPR Data Erasure](../master/Level3/.md)
- [ ] [Login Amy](../master/Level3/.md)
- [ ] [Login Bender](../master/Level3/.md)
- [ ] [Login Jim](../master/Level3/.md)
- [ ] [Manipulate Basket](../master/Level3/.md)
- [ ] [Payback Time](../master/Level3/.md)
- [ ] [Privacy Policy Inspection](../master/Level3/.md)
- [ ] [Product Tampering](../master/Level3/.md)
- [ ] [Reset Jim's Password](../master/Level3/.md)
- [ ] [Upload Size](../master/Level3/.md)
- [x] [Upload Type](../master/Level3/upload-type.md)
- [x] [XXE Data Access](../master/Level3/xxe-data-access.md)
