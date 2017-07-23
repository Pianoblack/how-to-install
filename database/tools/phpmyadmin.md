# MySQL installation

## Requirements

1. [PHP](../../language/php.md)
2. [MySQL](../mysql.md) or [MariaDB](../mariadb.md)

## Installation

### Linux

Login as root

```bash
> sudo su -
# Type root password
```

#### Ubuntu & Debian

Update packages and repositories

```bash
> apt-get update && apt-get upgrade
```

Install MySQL

```bash
> apt-get install phpmyadmin php-mbstring php-gettext
```

- You'll see a prompt for server selection. You must select your server with space key. You can switch with tab key if you want select another option
- Select yes when asked whether to use dbconfig-common to set up the database.
- You will be prompted for your database administrator's password
- You will then be asked to choose and confirm a password for the phpMyAdmin application itself

Restart your server

```bash
> systemctl restart apache2 # for apache2
> systemctl restart nginx # for nginx
```
