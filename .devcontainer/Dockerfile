# [Choice] Ubuntu version: bionic, focal
ARG VARIANT=bionic
FROM mcr.microsoft.com/vscode/devcontainers/base:${VARIANT}

# Install packages
RUN apt-get update 
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN apt-get install -y git
RUN apt-get install sqlite3
RUN apt-get clean

# Install python packages
RUN pip3 install web.py==0.51
