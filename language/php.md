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

#### Ubuntu

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
