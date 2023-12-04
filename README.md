# Hey! I'm Filing Here
UID: 605-691-763

In this lab, I successfully implemented a 1 MiB ext2 file system containing: 2 directories (root_directory, lost+found), 1 regular file (hello-world), and 1 symbolic link (hello->hello-world).

## Building

run 'make clean' if needed
run 'make'
run './ext2-create' to create the image 



## Running

run 'fsck.ext2 cs111-base.img' to ensure file system is correct
run 'dumpe2fs cs111-base.img' to get info about the file system
run 'mkdir mnt' to set up mounting point for image
run 'sudo mount -o loop cs111-base.img mnt' to mount the filesystem 
run 'cd mnt' to enter the directory
run 'ls -ain' to get detailed info about files + directories
run 'cat hello-world'  or 'cat hello' to output "Hello world\n" which is the contents of file 'hello-world'


## Cleaning up

run 'make clean'
run 'sudo umount mnt' to unmount the image
