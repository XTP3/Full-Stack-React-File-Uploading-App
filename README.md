# About
A full-stack headless file uploading web-app using NodeJS, React, and Express.

## Installation
### Server
#### Requirements
- NodeJS
- TLS/SSL Certificates (recommended)

Clone or Download the server's files and modify the Config.json accordingly.

Note: If you are using LetsEncrypt/Certbot you will need to set a filepath for the private key, certificate, and certificate authority (CA).
Note: File upload size is the maximum ALLOTTED file size permitted in one upload request, this means that the amount of files uploaded is irrelevant so long as they are beneath your limit size (in bytes).
