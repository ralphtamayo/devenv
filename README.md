# Development Environment
A docker development environment with MySQL 8.0, phpMyAdmin, and Nginx that currently supports React and Flask apps.

### How to use
1. Install Docker and Docker Compose.
2. Run `docker-compose up -d`

### MySQL
Default user is `root` with no password.

#### Commands
1. Restore database from a file.
    ```
    $ ./mysql/restore <db_name> <source>
    ```

2. Dump database to a file.
    ```
    $ ./mysql/dump <db_name> <destination>
    ```

### Nginx
#### Commands
1. Adding virtual host for React Apps.
    ```
    $ ./nginx/add-host react <app_name>
    ```

2. Adding virtual host for Flask Apps.
    ```
    $ ./nginx/add-host flask <app_name>
    ```