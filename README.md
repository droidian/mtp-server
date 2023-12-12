# MTP-Server - Small Server Implementation of Media Transfer Protocol
MTP allows media files to be transferred automatically to and from portable devices. Droidian includes `mtp-server` for Managig MTP. Some of the features are: 

* Fast and Easy-to-use File Transformation  
* No risk of file system corruption
* Mislocation

## Dependencies 
`mtp-server` requires the following development libraries:
- libboost-dev
- libboost-thread-dev
- libboost-filesystem-dev
- libboost-test-dev
- libandroid-properties-dev
- libgoogle-glog-dev
- libproperties-cpp-dev

## Manual Installation 
the `mtp-server` is implemented into the Droidian by default, but you can simply update or reinstall it by running 
```
$ sudo apt-get install mtp-server 
```

## Building 
```
$ git clone https://github.com/droidian/mtp-server.git
$ cd mtp-server
$ make
$ make install
$ dpkg-deb build mtp-server
```


The `mtp-server.service` should be enabled for starting itself during every boot: 
```
$ sudo systemctl enable --now mtp-server
```
