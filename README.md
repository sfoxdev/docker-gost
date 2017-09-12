# Gost - GO Simple Tunnel

A simple security tunnel written in Golang

[![Docker Build Status](https://img.shields.io/docker/build/sfoxdev/gost.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/automated/sfoxdev/gost.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/pulls/sfoxdev/gost.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/stars/sfoxdev/gost.svg?style=flat-square)]()

## Usage

### Run container
```
docker run -d -p 3128:3128 --name gost sfoxdev/gost -D -L=:3128 -F=example.com:3128
```

### Socks5 Auth

Server side
```
docker run -d -p 3128:3128 --name gost-srv sfoxdev/gost -D -L=socks5://tester:tester123@:3128
```

Client side
```
docker run -d -p 3128:3128 --name gost sfoxdev/gost -D -L=tester:tester123@:3128 -F=socks://tester:tester123@85.10.200.186:3128
```
