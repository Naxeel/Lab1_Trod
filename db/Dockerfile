FROM postgres:16

ENV POSTGRES_USER=app_user \
    POSTGRES_PASSWORD=app_password \
    POSTGRES_DB=app_db

COPY init.sql /docker-entrypoint-initdb.d/init.sql

