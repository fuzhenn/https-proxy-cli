# https-proxy-cli [![Build Status](https://travis-ci.org/naugtur/https-proxy-cli.svg?branch=master)](https://travis-ci.org/naugtur/https-proxy-cli)

[![Greenkeeper badge](https://badges.greenkeeper.io/naugtur/https-proxy-cli.svg)](https://greenkeeper.io/)

One command to run a local https proxy.

No need to set up certs!

## Install

```
npm install -g https-proxy-cli
```

## Usage

```
https-proxy -t http://localhost:80
```

```
https-proxy --help

Put https in front of your running app
Example: https-proxy -t http://localhost:8080 -p 8888 --path ~
Usage: https-proxy <options>

Options:
  -t, --target  target address, like http://localhost:80  [required]
  -p, --port    port to use for https                     [default: 3000]
  --keys        path for storing .key.pem and .cert.pem   [string]  [default: "."]
  --insecure    flag to accept insecure connections
  --xfwd        adds x-forward headers
  --cors                    set response header Access-Control-Allow-Origin to *
  --rewrite-origin          changes the origin of the host header to the target URL                                          [default: false]
  --rewrite-location        rewrites the location host/port on (201/301/302/307/308) redirects based on requested host/port  [default: false]
  --rewrite-cookies-domain  rewrites domain of set-cookie headers                                                            [default: false]
```
