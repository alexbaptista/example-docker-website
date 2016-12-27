Instructions for Project (example Docker Website)
========================================

## About

Docker Debian Wheezy (7) image, customized to be a Web server (Apache), aims to display a simple html that displays shortcuts to the Twitter project repositories `https://github.com/twitter/twitter.github`

## Setting up your local machine

* Install [Docker] (https://www.docker.com/products/overview)
* Clone this repo `https://github.com/cs-alex-baptista/example-docker-website`

## <i class="icon-download"></i> Configure your environment

* Access the project and build the Dockerfile

```
CD example-docker-website
docker build -t csalexbaptista/apache_webserver:latest .
```

* Run the new image and access from your local machine `localhost:80`

```
docker run --name debian7_webserver -d -ti -p 80:80 csalexbaptista/apache_webserver:latest
```

* Access bash

```
docker exec -ti debian7_webserver /bin/bash
```

## Troubleshooting

* Doc [Docker] (https://forums.docker.com/)
