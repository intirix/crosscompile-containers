# mingw-builds

Linux Dockerfiles that build windows binaries using mingw.  The goal is to use Dockerfiles
as the documentation of how to build various projects using mingw.


## Crypto++

Compile the latest Crypto++ to create a libcryptopp.a file

1. sudo docker build -t xcompile-cryptopp:latest -f crypto++.docker .
2. sudo docker run --rm -v $(pwd):/output xcompile-cryptopp:latest
