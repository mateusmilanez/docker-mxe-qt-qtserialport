# docker-mxe-qt-qtserialport


This repository have a Dockerfile that extends the docker image [yshurik/mxe-qt:gcc7](https://github.com/yshurik/docker-mxe-qt), this upgrade supports the qtserialport module.

To build the docker image use:
```
docker build -t docker-mxe-qt-qtserialport:latest .
```
To run your application:
```
docker run --rm -ti -v $(pwd):/app docker-mxe-qt-qtserialport:latest i686-w64-mingw32.static-qmake-qt5 && make
```
