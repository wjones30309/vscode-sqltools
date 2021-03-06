
# MySQL Start Guide

## 1. Connections

Connection example:
```json
{
  "name": "PGSQL",
  "server": "localhost",
  "dialect": "MySQL",
  "port": 3306,
  "database": "test_db",
  "username": "root",
  "askForPassword": false,
  "password": "root",
  "connectionTimeout": 15
}
```

### 1.1 Specific Options

MySQL driver specific options can be passed using `mysqlOptions` settings.

```json
{
  "name": "PGSQL",
  "server": "localhost",
  "dialect": "MySQL",
  "port": 5433,
  "database": "test_db",
  "username": "root",
  "askForPassword": false,
  "password": "root",
  "connectionTimeout": 15,
  "mysqlOptions": {
    ... // options
  }
}
```

| Option key  | Default Value | Allowed Values |
| ------------- | ------------- | ------------- |
| ssl  | `null`  | See section [SSL](#2-ssl) |



### 2. SSL

If you are using default protocol, see:

https://www.npmjs.com/package/mysql#ssl-options


If you are connecting using XProtocol, see:

https://dev.mysql.com/doc/dev/connector-nodejs/8.0/tutorial-Secure_Sessions.html

