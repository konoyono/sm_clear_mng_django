FROM python:3.7.2
ENV LANG en_US.utf8
WORKDIR /code
ADD requirements.txt /code
RUN apt-get update
RUN pip install -r requirements.txt
RUN apt-get install -y mysql-client
COPY ./docker-entrypoint.sh /
ENTRYPOINT ["/docker-entrypoint.sh"]