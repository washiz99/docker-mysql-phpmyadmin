# docker-mysql-phpmyadmin
Run MySQL and PHPMyAdmin on Docker

- docker 19.03.5
- docker-compose 1.24.0

## Instration

### 1. git clone 

```
$ docker clone https://github.com/washiz99/docker-mysql-phpmyadmin.git
```

### 2. edit .env file

```
$ cd docker-mysql-phpmyadmin
$ vim .env
```

| Key | Value | Desc |
| --- | --- | --- |
| MYSQL_HOST | mysql | MySQL Hostname |  
| MYSQL_DATABASE | testdb | Database name |
| MYSQL_ROOT_USER | root | root user |
| MYSQL_ROOT_PASSWORD | mysql | root password |
| MYSQL_USER | devuser | power user |
| MYSQL_PASSWORD | devuser | power user password |

## Usage

### Start

```
$ docker-compose up -d
```

### Terminate

```
$ docker-compose down
```

### access to phpadmin

1. Access to http://localhost:8080 with a browser(chrome/firefox/...).

```
http://localhost:8080
```

2. Login by entering the following contents.

- Server
  - Value specified for MYSQL_HOST (see above)
- Username
  - Value specified for MYSQL_ROOT_USER or MYSQL_USER (see above)
- Password
  - Value specified for MYSQL_ROOT_PASSWORD or MYSQL_PASSWORD (see above)

