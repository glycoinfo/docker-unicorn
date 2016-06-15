# Dockerfile
FROM postgres:9.5

RUN mkdir -p /tmp/psql_data/

COPY db/unicorn.sql /tmp/psql_data/
# COPY scripts/init_docker_postgres.sh /docker-entrypoint-initdb.d/
RUN /etc/init.d/postgresql start && /usr/bin/psql -a < /tmp/psql_data/unicorn.sql
