# gopeed-mipsel
```
go 1.22.2
flulter 3.16.0
```
```
sudo apt-get install gccgo-mipsel-linux-gnu
```
```
export GOARCH=mipsle
export GOOS=linux
export CGO_ENABLED=0
export CC=mipsel-linux-gnu-gcc
export CXX=mipsel-linux-gnu-g++
```
```
go build -tags nosqlite,web -ldflags="-s -w" -o bin/ github.com/GopeedLab/gopeed/cmd/web
```
![image](https://github.com/user-attachments/assets/6abe469c-5287-4b8e-a6e8-7f9f8e3e33f4)
