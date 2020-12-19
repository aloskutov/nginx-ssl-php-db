# nginx-ssl-php-mariadb
localhost nginx + SSL + php + mariadb + adminer

# Folders
## conf /
Configuration files

### conf / cert
Certificates
<pre>
localhost.crt
localhost.key
</pre>

### conf / mariadb
MariaDB configuration file
<pre>my.cnf</pre>

### conf / nginx
Nginx configuration file
<pre>localhost.conf</pre>

### conf / php
PHP configuration file
<pre>php.ini</pre>

## logs /
Log files
### logs / mariadb
<pre>mariadb.err</pre>
### logs / nginx
<pre>
access.log
error.log
</pre>

### logs / php
<pre>
errors.log
</pre>
## logs / mariadb
MariaDB database files

## src /
Source codes

# SSL for localhost

Install openssl.

<code lang='bash'>
choco install openssl
</code>

- [How to Get HTTPS Working in Windows 10 Localhost Dev Environment](https://zeropointdevelopment.com/how-to-get-https-working-in-windows-10-localhost-dev-environment/)
- [How to create an HTTPS certificate for localhost domains](https://gist.github.com/cecilemuller/9492b848eb8fe46d462abeb26656c4f8)
- [How to setup Let's Encrypt for Nginx on Ubuntu 18.04 (including IPv6, HTTP/2 and A+ SLL rating)](https://gist.github.com/cecilemuller/a26737699a7e70a7093d4dc115915de8)
