# gopeed-mipsel

sudo apt-get install gccgo-mipsel-linux-gnu

export GOARCH=mipsle
export GOOS=linux
export CGO_ENABLED=0
export CC=mipsel-linux-gnu-gcc
export CXX=mipsel-linux-gnu-g++

go build -tags nosqlite,web -ldflags="-s -w" -o bin/ github.com/GopeedLab/gopeed/cmd/web

![image](https://github.com/user-attachments/assets/200303da-1865-4e40-b373-704f96c8e39e)
