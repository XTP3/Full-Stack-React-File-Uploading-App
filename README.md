# About
This is a full-stack, headless, file-uploading web-application using React and Express.

## Installation
### Server
#### Requirements
- NodeJS
- TLS/SSL Certificates (recommended)

Clone or Download the server's files and modify the Config.json accordingly.

```
{
    "HTTP_PORT": 80,
    "HTTPS_PORT": 443,
    "PRIVATE_KEY_FILEPATH": "/some/folder/server.key",
    "CERTIFICATE_FILEPATH": "/some/folder/server.cert",
    "CA_CERT_FILEPATH": "",
    "PEM_PASSPHRASE": "",
    "DATABASE_URL": "mongodb://localhost/DatabaseName",
    "ACCOUNT_CREATION_CODE": "someRandomCode",
    "BCRYPT_SALT_ROUNDS": 10,
    "JWT_SECRET_KEY": "someRandomCode",
    "JWT_EXPIRATION": "30m",
    "MAX_UPLOAD_SIZE": 10737418240,
    "DATE_LANGUAGE": "en-US",
    "DATE_TIMEZONE_REGION": "America/New_York"
}
```

- Note: If you are using LetsEncrypt/Certbot you will need to set a filepath for the private key, certificate, and certificate authority (CA).
- Note: File upload size is the maximum ALLOTTED file size permitted in one upload request, this means that the amount of files uploaded is irrelevant so long as they are equal to or beneath your limit size (in bytes).

### Client
#### Requirements
- NodeJS

You will need to modify the front-end React Application and manually compile prior to deployment, as the configuration file is unaccessable during production.

Although not required, you may modify your HTML title in the /public directory by modifying index.html:

```
<title>Website Title</title>
```
