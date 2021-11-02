FROM python:3.7

ENV TZ=Asia/Almaty

COPY Pipfile* /tmp
RUN pip install pipenv
RUN cd /tmp && pipenv install --deploy

RUN mkdir /app
ADD . /app
WORKDIR /app
