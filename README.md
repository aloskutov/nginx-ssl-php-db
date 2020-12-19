# nginx-ssl-php-mariadb
localhost nginx + SSL + php + mariadb + adminer

## Project tree

<pre>
├───conf
│   ├───certs
│   ├───mariadb
│   ├───nginx
│   └───php
├───logs
│   ├───mariadb
│   ├───nginx
│   └───php
├───mariadb
└───src
</pre>


## Images
+ [PHP:fpm](https://hub.docker.com/_/php)
+ [MariaDB](https://hub.docker.com/_/mariadb)
+ [Nginx](https://hub.docker.com/_/nginx)
+ [Adminer](https://hub.docker.com/_/adminer)

This project use the following ports:

| Server     | Port |
|------------|------|
| MariaDB    | 3306 |
| Adminer    | 8080 |
| Nginx      |   80 |
| Nginx SSL  |  433 |
| PHP-FPM    | 9000 |


# SSL for localhost

Install mkcert.

```shell
choco install mkcert
```
Install RootCA
```
mkcert -install
```

Create certificates for localhost (or other hostname)
```
mkcert localhost
```

Copy them to /conf/certs and change nginx [config](conf/nginx/localhost.conf) options <code>ssl_certificate</code> and <code>ssl_certificate_key</code>

## Set localhost certificates in Firefox

Manually install the rootCA in firefox through firefox's cert manager (If it is not listed). Prefences -> Privacy & Security -> Certificates -> View Certificates -> Authorities (Tab) -> Import

Select certificate and set trust settings "Edit Trust..." -> set "This certificate can identify websites." -> ok


- [How to Get HTTPS Working in Windows 10 Localhost Dev Environment](https://zeropointdevelopment.com/how-to-get-https-working-in-windows-10-localhost-dev-environment/)
- [How to create an HTTPS certificate for localhost domains](https://gist.github.com/cecilemuller/9492b848eb8fe46d462abeb26656c4f8)
- [How to setup Let's Encrypt for Nginx on Ubuntu 18.04 (including IPv6, HTTP/2 and A+ SLL rating)](https://gist.github.com/cecilemuller/a26737699a7e70a7093d4dc115915de8)
