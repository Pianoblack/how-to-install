# Wordpress installation

## Requirements

- [PHP](../../language/php.md)
- [MySQL](../../database/mysql.md)
- [Nginx](../../web/server/nginx.md) or [Apache](../../web/server/apache.md)

## Installation

### Via FTP

1. Download latest wordpress release from [wordpress.org](https://wordpress.org)
2. Extract downloaded wordpress release
3. Login your server via FTP account
4. Upload extracted wordpress/* files to your server
5. Rename wp-cofig-sample.php to wp-config.php
6. Edit these lines in wp-config.php like below

```php
define('DB_NAME', 'YOUR_DATABASE_NAME');

/** MySQL database username */
define('DB_USER', 'YOUR_DATABASE_USER');

/** MySQL database password */
define('DB_PASSWORD', 'YOUR_DATABASE_PASSWORD');
```

### Via SSH

1. Login your server via SSH
2. Navigate to your domain directory (`cd /home/USERNAME/web/public_html` or `/var/www/html...` - maybe somethings different for you)
3. Run this commands

```bash
> wget https://wordpress.org/latest.tar.gz
> tar -xzvf latest.tar.gz 
> mv wordpress/* ./
> mv wp-config-sample.php wp-config.php
```

4. Edit these lines in wp-config.php like below

```php
define('DB_NAME', 'YOUR_DATABASE_NAME');

/** MySQL database username */
define('DB_USER', 'YOUR_DATABASE_USER');

/** MySQL database password */
define('DB_PASSWORD', 'YOUR_DATABASE_PASSWORD');
```
### Cheers!

Navigate to your domain with browser and install your wordpress site.
