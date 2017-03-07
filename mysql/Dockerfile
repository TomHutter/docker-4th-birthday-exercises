FROM mysql:5
COPY redmine.dmp.sql /docker-entrypoint-initdb.d/
# modified docker-entrypoint.sh with CREATE USER '$MYSQL_USER'@'%.%'
COPY docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh
