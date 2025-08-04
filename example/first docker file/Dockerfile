FROM ubuntu:latest
#set the working directory
WORKDIR /app

#copy the file to from working directrory

COPY ./app

#install the required pacages

RUN apt-get update && apt-get install -y python3 python3-pip

#set the environment varables
ENV NAME kiran

#runthe application

CMD ["python3", "app.py"]
