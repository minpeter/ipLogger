# ipLogger

[![Go Report Card](https://goreportcard.com/badge/github.com/minpeter/iplogger)](https://goreportcard.com/report/github.com/minpeter/iplogger)
[![Go Reference](https://pkg.go.dev/badge/github.com/minpeter/iplogger.svg)](https://pkg.go.dev/github.com/minpeter/iplogger)
[![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/minpeter/iplogger)](https://hub.docker.com/r/minpeter/iplogger)
[![Docker Pulls](https://img.shields.io/docker/pulls/minpeter/iplogger)](https://hub.docker.com/r/minpeter/iplogger)  
๐ Project What is my IP?

## purpose

A study on how services located behind multiple reverse proxies log real client IPs.

์ฌ๋ฌ ๋ฆฌ๋ฒ์ค ํ๋ก์ ๋ค์ ์์นํ ์๋น์ค๊ฐ ์ค์  ํด๋ผ์ด์ธํธ IP๋ฅผ ๊ธฐ๋กํ๋ ๋ฐฉ๋ฒ์ ๋ํ ์ฐ๊ตฌ

## screenshot

[![image](https://user-images.githubusercontent.com/62207008/217578966-c1daa0b2-5040-4906-abe8-aa7a2f276956.png)](https://ip.minpeter.cf)

## how to use?

```sh
$ curl ip.minpeter.cf -L
```

or <https://ip.minpeter.cf>

## deployment

with docker

```
$ docker build -t iplogger .
$ docker run -dp 10000:10000 iplogger
```

with golang

```
$ go mod tidy
$ go run .
```

now running on <http://localhost:10000>

## โจ result post (Korean) โจ

ํ๋ก์ ํธ์ ๋ํ ๊ฐ๋จํ [์ค๋ช ๊ธ](docs/result.md)

์ด ํ๋ก์ ํธ๋ฅผ ์งํํ๋ฉด์ ์์ฑํ [๋ธ๋ก๊ทธ ๊ธ](https://minpeter.github.io/uncategorized/%EB%B0%B1%EC%97%94%EB%93%9C%EC%97%90%EC%84%9C-client%EC%9D%98-ip%EB%A5%BC-%EB%A1%9C%EA%B9%85%ED%95%98%EB%8A%94-%EB%B0%A9%EB%B2%95)
