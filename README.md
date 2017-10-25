# hello-flask
Just a hello world app to test container as a service with.

## running locally

set up virtualenv (one time only):

    virtualenv -p python3 LOCAL

source it

    source LOCAL/bin/activate

install the python library requirements

    pip install -r requirements.txt 

run it

    export FLASK_APP=hello.py
    flask run

try it!

     curl -v http://127.0.0.1:5000/

## running in a container

build image

    docker build -t hello-flask .

run the container

    docker run -d -p 5000:5000 hello-flask:latest

start container and poke around

    docker run -t -i hello-flask:latest /bin/bash