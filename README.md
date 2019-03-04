# wscat

WebSocket cat.

## Installation

This module needs to be installed globally so use the `-g` flag when installing:

```
npm install -g https://github.com/barchart/wscat.git
```

## Usage

```
$ wscat -c ws://echo.websocket.org 
connected (press CTRL+C to quit)
> hi there
< hi there
> are you a happy parrot?
< are you a happy parrot?
```

## Chain Commands

`-w {x}` will keep the connection open for {x} seconds.

```
wscat -c wss://wsqs-e-barchart.aws.barchart.com/jerq \
  -x "login user:pass" \
  -x "ver 4" \
  -x "go ZCBG19NCSC.CM" \
  -w 10
```

## License

MIT
