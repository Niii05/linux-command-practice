# Day 4 - Networking Basics

## Commands Learned

ping google.com
→ Checks internet connectivity

curl localhost:8080
→ Sends request to local server

ss -tuln
→ Shows open ports and listening services

## Key Concepts

Network = Communication between systems

localhost = Your own machine

127.0.0.1 = Same as localhost

Port = Entry point for network requests

## Port Understanding

Port is like a gate through which requests enter a system

Examples:
80 → HTTP (web server)
443 → HTTPS (secure web)
8080 → custom applications

## Docker Networking

docker run -p 8080:80 nginx

Meaning:
Host Port: 8080
Container Port: 80

## Request Flow

Browser (localhost:8080)
↓
Host Port 8080
↓
Docker
↓
Container Port 80
↓
Nginx Service
↓
Response (HTML)

## Observations

* If container is not running → no response
* If port is not open → request fails
* curl can be used instead of browser
* localhost and 127.0.0.1 give same result

## Debugging Steps

1. Check container is running → docker ps
2. Check port mapping → docker run -p
3. Check service → nginx running
4. Use curl to test response

## What I Understood

* Network helps communication between browser and services
* Port is required to access services
* Docker connects host and container through port mapping
* Debugging network issues is important in DevOps

## Real Life Use

* Website not loading → check port and service
* Debug server issues using curl and logs
* Connect applications running in containers
