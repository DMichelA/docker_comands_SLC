# Download base image ubuntu 20.04
FROM ubuntu:20.04

# LABEL about the custom image
LABEL description = "Imagen para desarrollar con webpy"
LABEL mainteiner = "Amairani DI"
LABEL version = "0.1"

# Define ENV files
ENV requirements /home/requirements.txt

# Copy requirements file 
COPY requirements.txt ${requirements}

# Install python packages
RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN apt-get install -y sqlite3

RUN pip3 install -r /home/requirements.txt