# VPN (PPTP) for RPi

This is a docker image with simple VPN (PPTP) server with authentication work on raspberry pi.


## Starting VPN server

To start VPN server as a docker container run:

````
docker un -d -e VPN_USER='yourlogin' -e VPN_PASS='yourpassword' --privileged --net=host json1416/rpi-pptp
````
Default auth is `username` and `password`

Set user and passwrod

```
ENV VPN_USER username
ENV VPN_PASS password
```
