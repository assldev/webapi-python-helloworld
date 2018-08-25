# Description
It's just a simple *hello-world web-api* app. You could use it as a *boilerplate* for your simple web-api/ui app.

# Dependencies
- Flask==0.10.1

# Configuration
- Port number: Update in app/hello.py.

# Run
I've created a Dockerfile so there's no need to install python. Although, you need to have docker installed on your machine.
 ```
 cd app/
 docker build -t webapi-python-helloworld .
 docker run -p 8080:8080 webapi-python-helloworld
 ```
PS - You need to put the appropriate port numbers with -p flag.

If you prefer to use docker-compose:
```
docker-compose build
docker-compose up
```
PS - You need to update the docker-compose.yml file with the appropriate port number.

In case you want to run it directly with python:
```
cd app/
pip install -r requirements.txt
python hello.py
 ```