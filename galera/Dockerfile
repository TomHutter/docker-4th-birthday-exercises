FROM colinmollenhour/mariadb-galera-swarm

# create /root/.my.cnf with correct PW
ARG MYSQL_ROOT_PASSWORD
COPY redmine.dmp.sql /docker-entrypoint-initdb.d
COPY my.cnf /root/.my.cnf
RUN sed -i "s/password=/password=${MYSQL_ROOT_PASSWORD}/" /root/.my.cnf
