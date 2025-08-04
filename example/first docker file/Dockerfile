from ubuntu:latest
#set the working directory
workdir /app

#copy the file to from working directrory

copy ./app

#install the required pacages

run apt-get update && apt-get install -y python3 python3-pip

#set the environment varables
env NAME kiran

#runthe application

cmd ["python3", "app.py]
