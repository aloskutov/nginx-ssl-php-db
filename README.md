# nginx-ssl-php-mariadb
localhost nginx + SSL + php + mariadb + adminer

# Containers

Run containers
```shell
docker compose up -d
```

Stop containers
```shell
docker compose down
```

# Folders
## [conf /](conf/)
Configuration files

### [conf / certs](conf/certs)
Certificates
<pre>
localhost.crt
localhost.key
</pre>

# SSL for localhost

Install openssl.

```shell
choco install openssl
```

- [How to Get HTTPS Working in Windows 10 Localhost Dev Environment](https://zeropointdevelopment.com/how-to-get-https-working-in-windows-10-localhost-dev-environment/)
- [How to create an HTTPS certificate for localhost domains](https://gist.github.com/cecilemuller/9492b848eb8fe46d462abeb26656c4f8)
- [How to setup Let's Encrypt for Nginx on Ubuntu 18.04 (including IPv6, HTTP/2 and A+ SLL rating)](https://gist.github.com/cecilemuller/a26737699a7e70a7093d4dc115915de8)
