# LyticLingo RestServer

## Needed .env files
You need a .env file which will provide some information to the program. You could also porvide the enviornment variables through the normal way of loading them.

The required enviornment variables are the following.
| Variable | Description |
|--|--|
| SYSTEMKEY | the main API-Key used by the AdminDashboard |
| IP | the ip the restserver should bind to |
| PORT | the port the restserver should bind to |
| DB_HOST | the address of the PostgreSQL server |
|DB_PORT| the port of the PostgreSQL server |
| DB_NAME | the name of the PostgreSQL database |
| DB_USER | the name of the user which should be used to connect |
| DB_PASSWORD | the password of the user which should be used to connect
 
An example .env file
```bash
# program setting
SYSTEMKEY = mySecureSystemKey
IP = 127.0.0.1
PORT = 8080

#db connection
DB_HOST = 127.0.0.1
DB_PORT = 5432
DB_NAME = lyticlingo
DB_USER = myDBUser
DB_PASSWORD = foobar
```

This will provide all needed info to get the restserver up and running.
Other variable you can set are the following.
| Variable    | Description |
| -------- | ------- |
| USE_ADMIN  | create a static admin account (not recommended) |
| ADMIN_NAME | name for the static admin account |
| ADMIN_PASSWORD    | password for the static admin account |
| DB_USE_TABLE_PREFIX | prefix all tables used by the restserver |
| DB_TABLE_PREFIX | the used prefix for the tables |
| DB_USE_SSL | should ssl be used to connect to the database|
