## Bjoern's Favorite Pet
### Reset the password of Bjoern's OWASP account via the Forgot Password mechanism with the original answer to his security question.
### Category: Broken Authentication

From the previous challenge, after hacking in to `/administration` panel using admin user. We have a list of Bjoern's emails login used for juice shop. Using the forget password function, there is one particular email login `bjoern@owasp.org` that asks the question `Name of your favorite pet?` 

Googling bjoern's favorite pet would reveal the answer to be `Zaya` in solutions page. Even though the intended solution is found in a talk given by Bjoern where he registers an account in Juiceshop with the answer to this forget password question. The key lesson here is never to use a forget password question that could be easily answered by doing basic recon and target research by anyone!