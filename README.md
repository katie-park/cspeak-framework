# cspeak-framework [![Build Status](https://travis-ci.org/jscd/cspeak-framework.svg?branch=master)](https://travis-ci.org/jscd/cspeak-framework)

This repo is a C++ framework for interacting with TeamSpeak's ServerQuery and ClientQuery interfaces.

## Building
Was build using both clang and gcc.

To build locally run:
```console
foo@bar:~$ mkdir build
foo@bar:~$ cd build
foo@bar:~$ cmake ..
foo@bar:~$ make
```

## Usage
To use you can include the `cspeak.h` header and link the libraries using the compiler of your choice.

## Built With
* [libssh](https://www.libssh.org) - Framework for SSH connections in C

## Authors
* **Justin DeSimpliciis** - *Initial & Ongoing Development* - [jscd](https://github.com/jscd)