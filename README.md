# gopeed-mipsel
![输入图片说明](https://images.gitee.com/uploads/images/2020/0329/060357_d50dc364_899222.jpeg "QQ截图20200329060210.jpg")
![输入图片说明](https://images.gitee.com/uploads/images/2020/0329/060408_475d69a4_899222.jpeg "QQ截图20200329060118.jpg")
 支持一下 :smile: 

 
https://github.com/GopeedLab/gopeed
```
Ubuntu 24.04 LTS
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
cd ui/flutter
flutter build web
cd ../../
rm -rf cmd/web/dist
cp -r ui/flutter/build/web cmd/web/dist
go build -tags nosqlite,web -ldflags="-s -w" -o bin/ github.com/GopeedLab/gopeed/cmd/web
```
```
后台运行:
chmod a+x gopeed-mipsel-1.5.8
(./gopeed-mipsel-1.5.8 &)
```
![image](https://github.com/user-attachments/assets/6ff055c9-8cd2-4c09-b3d6-4b5464b2a1fb)
![image](https://github.com/user-attachments/assets/1eb75ab2-a716-4d2c-a3d3-99ee9cd33435)

