FROM ubuntu:latest

WORKDIR /usr/src/app

RUN apt-get update
RUN apt-get install python3 python3-pip -y

RUN pip3 install flask flask_cors flask_sqlalchemy boto3 requests pymysql pillow python-openam
