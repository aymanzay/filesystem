CSE303 - Fall 2017
Assignment #3: Filesystems

Purpose and General Guidelines:

  It is reasonable to think of a filesystem as being nothing more than a data structure. The operations of that data structure can vary\
, depending on the operating system. They may also have different asymptotic complexities, and filesystem methods may have different me\
anings on an OS-by-OS basis. A few examples are that (a) UNIX filesystems support the concept of reference-counted "hard links", wherea\
s NTFS does not; (b) the MS-DOS FAT filesystem exposes a "seek" operation that is linear in the size of the file, whereas UNIX filesyst\
ems expose a "seek" operation that is logarithmic in the size of the file; and (c) UNIX filesystems require the 'accessed time' to be u\
pdated when a file is read, resulting in a disk write of file metadata even when the file contents are in the cache.

In this project, we will be creating a high-level API for a filesystem that you design under our requirements.
