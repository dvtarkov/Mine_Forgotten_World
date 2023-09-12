FROM python:3.11

ENV PYTHONUNBUFFERED=1

WORKDIR /srv/www/mine_forgotten

RUN apt-get update -y && apt-get upgrade -y

COPY ./mine_forgotten/requirements.txt requirements.txt

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

COPY ./mine_forgotten /srv/www/mine_forgotten

COPY prod.env prod.env
