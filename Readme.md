nginx-simple-proxy
==================


A dead simple docker image to implement proxy to a different path


    docker run -it -e NGINX_PORT=80 -e SERVERNAME=server -e PROXY_PASS=http://mybuildbot:8020/hooks -p 8080:80 nginx-simple-proxy

Meant to be used to avoid opening a full buildbot to the internet.
