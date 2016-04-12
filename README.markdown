# pianobarproxy
--
Command pianobarproxy is a simple SOCKS5 shim for pianobar.

This lets you proxy pianobar through ssh (or any SOCKS5 provider).

    # Start your SOCKS5 proxy via ssh:
    ssh -v -D localhost:9080 -C -N example.com

    # Start pianobarproxy:
    pianobarproxy -socks5 :9080

    # Add the following to $HOME/.config/pianobar/config:
    proxy = http://localhost:9090

### Install

    go get github.com/stevenirby/pianobarproxy


### Usage

    Usage of pianobarproxy:
        -listen="localhost:9090": The listening address
        -socks5="localhost:1080": The address of the SOCKS5 proxy

