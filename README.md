# sysfs-module-template
## Usage
```
$ make
$ sudo insmod sysfs.ko
$ dmesg | grep hello
[ 7951.629147] hello sysfs module
$ ls -l /sys/module/sysfs/fooattrs
total 0
-r--r--r-- 1 root root 4096 Nov 16 23:49 name
-rw-r--r-- 1 root root 4096 Nov 16 23:49 value
$ cat /sys/module/sysfs/fooattrs/name
sysfs-moduld
$ cat /sys/module/sysfs/fooattrs/value
0
```
