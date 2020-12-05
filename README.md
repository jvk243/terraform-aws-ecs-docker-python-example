# terraform-aws-ecs-docker-python-example

Simple example of integrating [docker](https://www.docker.com/) with web apps, [flask](http://flask.pocoo.org/) in this case

## Running it


**NOTE**: Command can vary depending on the OS you are on

Pull my docker image

```sh
$ docker pull xxxx/flask-example
```

Run the flask app

```sh
$ docker run -p 5000:5000 xxxx/flask-example
* Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
```

You will find the running app instance at [http://localhost:5000/](http://localhost:5000/)

![app on localhost](http://i.imgur.com/5pJ41n1.png)

## Building the `Dockerfile` locally

If you are feeling pumped for the day, you can build the `Dockerfile` locally.

```sh
$ git clone https://github.com/jvk243/terraform-aws-ecs-docker-python-example.git && cd docker-flask
$ docker build -t flask_docker .
$ docker run -p 5000:5000 flask_docker
# open the app on http://localhost:5000/
```
