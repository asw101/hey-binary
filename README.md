# README

A simple repo for @rakyll's fantastic 'hey' tool: <https://github.com/rakyll/hey>

The best way to install is to simply [download go](https://golang.org/dl/), go get and add to path.

I'm also cross-compiling some binaries which can be [downloaded from this repo](https://github.com/asw101/hey-binary/releases).
## go get

    go get -u github.com/rakyll/hey
    echo 'export PATH=$PATH:~/go/bin' >> ~/.bash_profile

## go build

    go get -u github.com/rakyll/hey
    mkdir ~/hey/
    cd  ~/go/src/github.com/rakyll/hey
    GOOS=windows GOARCH=amd64 go build -o ~/hey/hey.exe hey.go
    GOOS=linux GOARCH=amd64 go build -o ~/hey/hey_linux hey.go
    GOOS=darwin GOARCH=amd64 go build -o ~/hey/hey_darwin hey.go
