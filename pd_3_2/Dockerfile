#mysql -h localhost -U myuser -p
FROM mysql:8.0

ENV MYSQL_ROOT_PASSWORD=rootpass \
    MYSQL_DATABASE=myapp \
    MYSQL_USER=myuser \
    MYSQL_PASSWORD=mypassword

# 2. Копируем SQL-дамп в специальную директорию
# Всё, что окажется в /docker-entrypoint-initdb.d будет выполнено при первом запуске
COPY init.sql /docker-entrypoint-initdb.d/

# 3. Документируем порт и том
EXPOSE 3306
VOLUME /var/lib/mysql