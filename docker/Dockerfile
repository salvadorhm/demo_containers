# Download base image ubuntu 18.04
FROM ubuntu:bionic

# LABEL about the custom image
LABEL maintainer="Salvador HM salvadorhm@gmail.com"
LABEL version="0.1"
LABEL description="This is a ubuntu:18.04 with web.py 0.51 and SQlite3 "

# Definbe ENV files
ENV requirements /home/requirements.txt

# Copy requirements file
COPY requirements.txt ${requirements}

# Install packages
RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN apt-get install -y git
RUN apt-get install sqlite3
RUN apt-get clean

# Install python packages
RUN pip3 install web.py==0.51
