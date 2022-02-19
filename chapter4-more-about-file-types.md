<h2> More about file types </h2>

Linux treat the file extension as "everything is a file"

For example if a file extension is jpeg or mp3 and if we want to know the file type then simply we can type " file filename "

lets download an image from web by 

`wget "https://cdn.quotesgram.com/img/64/68/871911642-Peace-Facebook-Covers-2063.jpeg"`

`ls`

`file 871911642-Peace-Facebook-Covers-2063.jpeg`

In output it will show the file is of type jpeg.

![image](https://user-images.githubusercontent.com/38061560/154790489-ecd522ef-57de-4777-8b1b-2f3b5ca203d6.png) 

Less Command
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
The Less command in linux is to View Text file and it also gives us scrolling files in a windows in any direction.

the less command syntax is - `less filename` .

it is only for viewing the text files.

type `less /etc/passwd`  and navigate up and down through the windows.

type `less libaudit.conf ` and search inside file by pressing `/ignore` and we can see "ignore" text in the file.
 
![image](https://user-images.githubusercontent.com/38061560/154791433-dc686ca6-f54d-4e60-b610-805695ee5ebd.png)

if we want to come out of windows , then press `q` to exit from the screen and coming back to terminal.

<h4> Less Is More </h4>
The less program was designed as an improved replacement of an earlier Unix
program called more. The name “less” is a play on the phrase “less is more” — a
motto of modernist architects and designers.

less falls into the class of programs called "pagers" programs that allow the
easy viewing of long text documents in a page by page manner.

Whereas the
more program could only page forward, the less program allows paging both
forward and backward and has many other features as well.

---------------------------------------------------------------------------------------------------------------------------------------------------------------
<h3> About Directories Found on Linux Systems. </h3>

Lets Start with Root ( / ) - Everything in Linux Start from Root.

1. cd / - we enter in root where all directories are been placed.

![image](https://user-images.githubusercontent.com/38061560/154792519-ce6fc9b1-4043-41ab-a64d-a41b18479722.png)

2. /bin - contains the binaries that must be present for the system to boot and run 

like we install package by `apt install apache1` , so here apt , apt-cache package manager  files are present which helps us to update and run the services smoothly.

also commands like cal,chmod,clear,curl, etc are present here in binary.


![image](https://user-images.githubusercontent.com/38061560/154794539-78c60fd4-8495-4109-be66-2a4d5fbcdbb5.png)

3. /boot - 
 It contains the Linux Kernel[vmlinuz-4.19.0-18-cloud-amd64 ] 
 
 initial RAM disk image [ initrd.img-4.19.0-18-cloud-amd64]
 
 and Boot Loader.

some files - /boot/grub/grub.conf or menu.1st which are used to configure the boot loader.

/boot/vmlinuz  ( or similar) the linux kernel file.

![image](https://user-images.githubusercontent.com/38061560/154795350-e60e2986-54b6-4189-aa49-2275250b3085.png)

inside grub.cfg file , there is instruction to load kernel image and ram when booting up system.
![image](https://user-images.githubusercontent.com/38061560/154796045-8dc8990f-404e-4ebe-b0cc-e874de3911bd.png)

as you can see it calls the image to be loaded .

linux /boot/vmlinuz-4.19.0-17-amd64 {
      initrd /boot/initrd.img-4.19.0-17-amd64
   }

![image](https://user-images.githubusercontent.com/38061560/154796340-cd72e26b-f47d-4bba-a354-94a7f02fc8fc.png)


