# MariaDB installation

If you have installed MySQL server your system, you can use these tools for connect and use.

1. [PhpMyAdmin](./tools/phpmyadmin.md)
2. [DBeaver](http://dbeaver.jkiss.org/download/)
4. [Datagrip](https://www.jetbrains.com/datagrip/download/)
3. [Sequel Pro](https://sequelpro.com/download)

You can search for more tools.

## Installation

### Linux

Login as root

```bash
> sudo su -
# Type root password
```

#### Ubuntu

Update packages and repositories

```bash
> apt-get update && apt-get upgrade
```

Add MariaDB repo to our system

```bash
> sudo apt-get install software-properties-common
> sudo apt-key adv --recv-keys --keyserver hkp://keyserver.ubuntu.com:80 0xF1656F24C74CD1D8
> sudo add-apt-repository 'deb [arch=amd64,i386,ppc64el] ftp://ftp.ulak.net.tr/pub/MariaDB/repo/10.2/ubuntu xenial main'
```

Install MariaDB

```bash
> apt-get update
> apt-get install mariadb-server
```

Start MariaDB

```bash
> systemctl start mariadb
> systemctl enable mariadb # enable autostart with session
```

MySQL secure installation

```bash
> mysql_secure_installation
# Answer the questions...
```

#### Debian

Update packages and repositories

```bash
> apt-get update && apt-get upgrade
```

Add MariaDB repo to our system

```bash
> sudo apt-get install software-properties-common
> sudo apt-key adv --recv-keys --keyserver keyserver.ubuntu.com 0xF1656F24C74CD1D8
> sudo add-apt-repository 'deb [arch=amd64] ftp://ftp.ulak.net.tr/pub/MariaDB/repo/10.2/debian stretch main'
```

Install MariaDB

```bash
> apt-get update
> apt-get install mariadb-server
```

Start MariaDB

```bash
> systemctl start mariadb
> systemctl enable mariadb # enable autostart with session
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

Install MariaDB

```bash
> dnf install mariadb-server
```

Start MariaDB server

```bash
> systemctl start mariadb
> systemctl enable mariadb # enable autostart with session
```

MySQL secure installation

```bash
> mysql_secure_installation
# Answer the questions...
```

### MacOS

We use brew for install MariaDB

```bash
> brew install mariadb
> mysql_install_db
```

Start MariaDB server

```bash
mysql.server start
```

MySQL secure installation

```bash
> /usr/local/bin/mysql_secure_installation
# Answer the questions...
```
