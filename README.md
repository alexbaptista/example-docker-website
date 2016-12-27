Instructions for Project (example Docker Website)
========================================

## About

Docker Debian Wheezy (7) image, customized to be a Web server (Apache), aims to display a simple html that displays shortcuts to the Twitter project repositories `https://github.com/twitter/twitter.github`

## Setting up your local machine

* Install [Docker] (https://www.docker.com/products/overview)
* Clone this repo `https://github.com/cs-alex-baptista/example-docker-website`

## Configure your environment

* Access the project and build the Dockerfile

```
CD example-docker-website
docker build -t csalexbaptista/apache_webserver:latest .
```

* Run the new image

```
docker run -ti -p 80:80 csalexbaptista/apache_webserver:latest /bin/bash
```

### Troubleshooting

* Doc [Docker] ()
