# Docker MySQL Shared

Docker compose setup for MySQL with intention of sharing it with multiple projects.

Note: This is meant to be used for development/testing machines only as you would likely use a bigger database setup in production like AWS RDS for example.

## Usage

Note: We are using a hardcoded root password here. This is because this is intended to be used in a development workflow. If you want a randomly generated password instead, read the instructions here: https://hub.docker.com/_/mysql/ to customize the docker build.

~~~
cd /path/do/docker-mysql-shared
sudo docker-compose up -d
~~~

## CLI Access

Note: Using a hardcoded root password.

~~~
mysql --port 3307 --protocol tcp -u root -pdarkstardb
~~~
