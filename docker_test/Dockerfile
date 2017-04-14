FROM ubuntu:latest
RUN apt-get update -y
RUN apt-get -y install python python-pip 
RUN pip install --upgrade pip
WORKDIR /code
ADD  . /code
RUN pip install -r requirements.txt
EXPOSE 8000
CMD python manage.py runserver 0.0.0.0:8000
