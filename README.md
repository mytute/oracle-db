# oracle-db

### install on ubuntu

1. first you need to download jdk to work with oracle

https://www.oracle.com/java/technologies/downloads/     


download deb file of jdk(here version 11) and install it.

```bash
$ sudo dpkg -i jdk-11.0.14_linux-x64_bin.deb
```

2. then download oracle sql and install

https://www.oracle.com/tools/downloads/sqldev-downloads.html    

```bash
$ sudo alien sqldeveloper-21.4.2-018.1706.noarch.rpm # conver rpm to deb
$ sudo alien -i sqldeveloper_21.4.2-19.1706_all.deb   # install converted deb file
```

this will install '/opt/sqldeveloper' by default.

to run oracle software

```bash
$ /opt/sqldeveloper  $ ./sqldeveloper.sh
```

3. make oracle direct start from cmd.   

```bash
$ sudo ln -s [YOUR_SQLDEVELOPER.SH_PATH] /usr/local/bin/sqldeveloper
$ sudo ln -s /opt/sqldeveloper/sqldeveloper.sh /usr/local/bin/sqldeveloper
```

to start oracle    
```bash
$ sudo sqldeveloper  
```    

### connect with Node

for this you should have oracle client in your machine.

if there any 32-64bit mismatch then install following packages for linux
```bash
sudo apt-get install libaio1 libaio-dev
```
