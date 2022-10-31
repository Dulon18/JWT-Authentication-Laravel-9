<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://miro.medium.com/max/788/1*XkmnsJ6Joa6EDFVGUw0tfA.png" width="400" alt="Laravel Logo"></a></p>


## What is JWT(JSON Web Token)?

JSON Web Token (JWT) is an open standard (RFC 7519), and it represents a compact and self-contained method for securely transmitting information between parties as a JSON object. Digital signature makes the data transmission via JWT trusted and verified. JWTs built upon the secret HMAC algorithm or a public/private key pair using RSA or ECDSA.

## Why is JWT Required?

JWT is used for Authorization and information exchange between server and client. It authenticates the incoming request and provides an additional security layer to REST API, which is best for security purposes.

## How does JWT Work?

User information such as username and password is sent to the web-server using HTTP GET and POST requests. The web server identifies the user information and generates a JWT token and sends it back to the client. Client store that token into the session and also set it to the header. On the next HTTP call, that token is verified by the server, which returns the response to the client.

## JSON Web Token Structure
JSON Web Tokens contains three parts separated by dots (.) In its dense form.

- Header
- Payload
- Signature

Eventually, a JWT similarly looks like this -> xxxxx.yyyyy.zzzzz

## Laravel JWT authentication vs. Sanctum or Passport
Choosing the type of authentication to use in your Laravel application is based on the type of application you’re building. Sanctum offers both session-based and token-based authentication and is good for single-page application (SPA) authentications. Passport uses JWT authentication as standard but also implements full OAuth 2.0 authorization.

OAuth allows authorization from third-party applications like Google, GitHub, and Facebook, but not every app requires this feature. If you want to implement token-based authentication that follows the JWT standard, but without the OAuth extras, then Laravel JWT authentication is your best bet.

## Package

- composer require php-open-source-saver/jwt-auth
- php artisan jwt:secret

## Installation Instructions
- Clone the repo.
- Run 'composer install'
- Run 'cp .env.example .env'
- Run 'php artisan migrate'
- Run 'php artisan serve'



## OUTPUT
<p align="center">
<img width="900px" src="https://user-images.githubusercontent.com/80118217/197402410-9ba0854f-b90e-484e-87b0-3ac47a5564f8.JPG">
</p>


<p align="center">
<img width="900px" src="https://user-images.githubusercontent.com/80118217/197402624-44b805db-2527-4641-b620-16cafd1a6c58.JPG">
</p>

<p align="center">
<img width="900px" src="https://user-images.githubusercontent.com/80118217/197403119-e122ae4c-3d75-468f-9eac-99ca4510f41b.JPG">
</p>


<p align="center"><span style="color: red;">&hearts;</span> Thank You <span style="color: red;">&hearts;</span></p>
