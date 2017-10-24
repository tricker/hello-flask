# hello-flask
Just a hello world app to test container as a service with.

## running locally

set up virtualenv (one time only):

`virtualenv -p python3 LOCAL`

source it

`source LOCAL/bin/activate`

install the python library requirements

`pip install flask`

run it

    export FLASK_APP=hello.py
    flask run

try it!

     curl -v http://127.0.0.1:5000/