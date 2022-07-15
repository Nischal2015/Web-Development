FROM python:3.8-alpine3.15

WORKDIR /usr/src/app

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

RUN apk add libpq-dev alpine-sdk libressl-dev libffi-dev && pip3 install --upgrade pip && pip3 install setuptools==45 wheel

COPY requirements.txt .

RUN pip install -r requirements.txt 

COPY . .

RUN python manage.py migrate