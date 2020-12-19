# nginx-ssl-php-mariadb
localhost nginx + SSL + php + mariadb + adminer

# Folders
## conf
Configuration files

### cert
Certificates
<code>
localhost.crt
localhost.key
</code>

### mariadb
MariaDB configuration file
<code>my.cnf</code>

### nginx
Nginx configuration file
<code>localhost.conf</code>

### php
PHP configuration file
<code>php.ini</code>

## logs
Log files
### mariadb
mariadb.err 
### nginx
access.log
error.log
### php
errors.log
## mariadb
MariaDB database files
## src
Source codes

## SSL for localhost

Install openssl.

<code lang='bash'>
choco install openssl
</code>

- [How to Get HTTPS Working in Windows 10 Localhost Dev Environment](https://zeropointdevelopment.com/how-to-get-https-working-in-windows-10-localhost-dev-environment/)
- [How to create an HTTPS certificate for localhost domains](https://gist.github.com/cecilemuller/9492b848eb8fe46d462abeb26656c4f8)
- [How to setup Let's Encrypt for Nginx on Ubuntu 18.04 (including IPv6, HTTP/2 and A+ SLL rating)](https://gist.github.com/cecilemuller/a26737699a7e70a7093d4dc115915de8)

## PHP

## Nginx

## MariaDB

## Adminer