FROM mysql:latest

#ENV MYSQL_ROOT_PASSWORD password
#ENV MYSQL_PASSWORD password
#ENV MYSQL_DATABASE databasename

# this need to stay the same for script to work
ENV MYSQL_USER mysql

COPY ./run.sh /
RUN chmod 755 /run.sh

ENTRYPOINT ["/run.sh"]
