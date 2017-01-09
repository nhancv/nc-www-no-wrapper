# nc-www-no-wrapper
remove www prefix

```xml
<VirtualHost *:80>
    ServerName www.nhancv.com
    DocumentRoot "this repository dir"
    <Directory "this repository dir">
        Options Indexes FollowSymLinks Includes execCGI
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>
```

###Usage
access if you access to www.nhancv.com it auto redirect to nhancv.com

- select with http
```bash
$ git checkout tags/http
```

- select with https
```bash
$ git checkout tags/https
```