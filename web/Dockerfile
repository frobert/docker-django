FROM python:3.7-slim

RUN apt-get update \
  && apt-get -y install libpq-dev gcc

RUN python -m pip install --upgrade pip

COPY requirements.txt requirements.txt
RUN python -m pip install -r requirements.txt

COPY . .
