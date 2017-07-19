# PHP Installation

For PHP 7.1

## Requirements

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

Install PHP

```bash
> apt-get install php7.1
```

Install PHP modules

```bash
> apt-cache search php7.1-*
# Choose and install like below
> apt-get install php7.1-mysql php7.1-curl php7.1-mbstring ...
```

#### Fedora

Update packages and repositories

```bash
> dnf update
```

Install PHP

```bash
> dnf install -y php-cli
```

Install PHP modules

```bash
> dnf search php-*
# Choose and install like below
> dnf install -y php-mysqli php-curl php-mbstring ...
```

### MacOS

#### Via [Brew](../cli-tools/osx/brew.md)

Tab required brews

```bash
> brew tap homebrew/homebrew-php
# Update brew
> brew update
```

Install PHP

```bash
> brew install php71
```

Install PHP modules

```bash
> brew search php71-
# Choose and install like below
> brew install php71-mysqli php71-curl php71-mbstring ...
```
