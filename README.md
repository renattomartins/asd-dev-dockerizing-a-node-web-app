# ASD - DEV - Dockerizing a node web app
A simple demo Docker+Node web app. This is a simple repository for future reference.

It was based in [Dockerizing a Node.js web app](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/) tutorial.

### Instructions to run the application
1. Clone this repository
2. Run the command `$ docker build -t <your username>/node-web-app .` on cloned project root folder.
3. See if ok with the command `$ docker images`, the name of your image must appear.
4. Run the command `docker run -p 49160:8080 -d <your username>/node-web-app` also on cloned project root folder.
5. After this, to test if all the things are ok, you must run `curl -i localhost:49160` and you will see:
> HTTP/1.1 200 OK<br>
> X-Powered-By: Express<br>
> Content-Type: text/html; charset=utf-8<br>
> Content-Length: 12<br>
> ETag: W/"c-M6tWOb/Y57lesdjQuHeB1P/qTV0"<br>
> Date: Sat, 13 Jan 2018 19:36:42 GMT<br>
> Connection: keep-alive<br>
><br>
> Hello world

## About the development environment
 - node v6.11.5
 - npm v5.6.0
 - docker 17.09.1-ce, build 19e2cf6
 - Git 2.14.1
 - GitHub
