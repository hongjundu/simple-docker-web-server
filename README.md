# Simple web server running in a docker container

## 1. Build nginx image
    docker build -t mynginx .

## 2. Run docker container as a web server
    docker run -d  -v /path/to/docker-nginx-web-server/web:/web -p 80:80 mynginx

## 3. Access web site hosted in the running docker container
    http://localhost