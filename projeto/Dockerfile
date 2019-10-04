FROM python:3.6
ENV PYTHONUNBUFFERED 1
RUN mkdir /projeto
WORKDIR /projeto
# Installing OS Dependencies
RUN apt-get update && apt-get upgrade -y && apt-get install -y \
libsqlite3-dev
RUN pip install -U pip setuptools
COPY requirements.txt /projeto/
RUN pip install -r /projeto/requirements.txt

ADD . /projeto/
# Django service
EXPOSE 8000
