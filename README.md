bootimgtools
=============

## A user-friendlier fork of the classic android-mkbootimg.

### Building

``
$ make
``

### Usage: unpackbootimg

```
$ ./unpackbootimg
usage: unpackbootimg
  -i|--input boot.img
  [ -o|--output output_directory]
  [ -p|--pagesize <size-in-hexadecimal> ]
  [ -n|--no-config ]
```

### Usage: mkbootimg

```
$ ./mkbootimg
usage: mkbootimg
       --imgdir <image-directory>
       -o|--output <filename>
```

### Usage: mkbootimg (without config file)

```
$ ./mkbootimg
usage: mkbootimg
       --kernel <filename>
       --no-config
       [ --ramdisk <filename> ]
       [ --second <2ndbootloader-filename> ]
       [ --cmdline <kernel-commandline> ]
       [ --board <boardname> ]
       [ --base <address> ]
       [ --pagesize <pagesize> ]
       [ --dt <filename> ]
       [ --kernel_offset <base offset> ]
       [ --ramdisk_offset <base offset> ]
       [ --second_offset <base offset> ]
       [ --tags_offset <base offset> ]
       [ --os_version <A.B.C version> ]
       [ --os_patch_level <YYYY-MM-DD date> ]
       [ --hash <sha1(default)|sha256> ]
       [ --id ]
       -o|--output <filename>
```



Credits to [@osm0sis](https://github.com/osm0sis/mkbootimg) for maintaining
most of the unpackbootimg logic that is no longer present in AOSP.
