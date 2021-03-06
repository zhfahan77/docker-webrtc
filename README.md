# WebRTCVideoChat

## Details

A Simple One to One Browser Based Video Chatting Application with features like,

* Login and Registration.
* Active User List

Technology used,

* [WebRTC](https://developer.mozilla.org/en-US/docs/Web/API/WebRTC_API)
* [Websocket](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API)
* [NodeJS](https://nodejs.org/en/)

WebRTC is a free, open project that provides browsers and mobile applications with Real-Time Communications (RTC) capabilities via simple APIs. The WebRTC components have been optimized to best serve this purpose.

### WebRTC Diagram

![WebRTC Diagram](https://www.html5rocks.com/en/tutorials/webrtc/infrastructure/jsep.png "WebRTC Diagram")

### WebSocket Diagram
![WebSocket Diagram](https://images.techhive.com/images/article/2016/06/websockets-100668229-primary.idge.jpg "WebSocket Diagram")

The WebSocket object provides the API for creating and managing a WebSocket connection to a server, as well as for sending and receiving data on the connection.

Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.

## Setup

In `public` dir, create a .env file, add your websocket server's IP

```
WEBSOCKET_IP=192.168.1.100
```

In root dir of the project, create a .env file to replace env variables if needed (To Run using node command)

```
dbURL=mongodb://<mongodb_host_ip>:<mongodb_port>/<database_name>
SECRET=<your_secret>
```


## Pre Requisits

* [Docker CE](https://docs.docker.com/install/linux/docker-ce/ubuntu/)
* [Docker Compose](https://docs.docker.com/compose/install/#install-compose)

## Start

### In Linux
```
make up
```

### In Windows
```
docker-compose up -d --build
```

## Down

### In Linux
```
make down
```

### In Windows
```
docker-compose down
```

## Build Only

### In Linux
```
make build
```

### In Windows
```
docker-compose build
```

## Remove Everything

### In Linux
```
make clean
```

### In Windows
```
docker-compose down -v
```

*Now you can access the application on https://localhost