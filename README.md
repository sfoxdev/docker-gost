# Gost - GO Simple Tunnel

A simple security tunnel written in Golang

[![Docker Build Status](https://img.shields.io/docker/build/sfoxdev/gost.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/automated/sfoxdev/gost.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/pulls/sfoxdev/gost.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/stars/sfoxdev/gost.svg?style=flat-square)]()

## Usage

### Run container
```
docker run -d --name gost sfoxdev/gost -D -L:3128 -F:example.com:3128
```
