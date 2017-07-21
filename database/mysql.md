# MySQL installation

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
> apt-get install mysql-server
```

Start MySQL server

```bash
> systemctl start mysqld
> systemctl enable mysqld # enable autostart with session
```

MySQL secure installation

```bash
> mysql_secure_installation
# Answer the questions...
```

#### Fedora

Update packages and repositories

```bash
> dnf update
```

Install MySQL

```bash
# Fedora 26
> dnf install https://dev.mysql.com/get/mysql57-community-release-fc26-10.noarch.rpm

# Fedora 25
> dnf install https://dev.mysql.com/get/mysql57-community-release-fc25-9.noarch.rpm

# Fedora 24
> dnf install https://dev.mysql.com/get/mysql57-community-release-fc24-9.noarch.rpm

# Fedora 23
> dnf install https://dev.mysql.com/get/mysql57-community-release-fc23-9.noarch.rpm

> dnf install mysql-community-server
```

Start MySQL server

```bash
> systemctl start mysqld
> systemctl enable mysqld # enable autostart with session
```

MySQL secure installation

```bash
> mysql_secure_installation
# Answer the questions...
```

### MacOS

Best way is use mariadb. Please checkout [mariadb installation instructions.](./mariadb.md)
