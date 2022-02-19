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

as you can see it calls the image to be loaded 

```

linux /boot/vmlinuz-4.19.0-17-amd64{
initrd /boot/initrd.img-4.19.0-17-amd64
 }

```

![image](https://user-images.githubusercontent.com/38061560/154796340-cd72e26b-f47d-4bba-a354-94a7f02fc8fc.png)

4. / dev 

Here the information about devices are being stored.

This is a special directory that contains device nodes.

The Kernel mantains a list of all the devices it understands.

The devices such that boot disks and non-boot disk are located here
as in below screenshot we can see the sda and its partision , sdb information is stored

```

NAME    MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
sda       8:0    0   10G  0 disk 
├─sda1    8:1    0  9.9G  0 part /
├─sda14   8:14   0    3M  0 part 
└─sda15   8:15   0  124M  0 part /boot/efi
sdb       8:16   0   17G  0 disk


root@sanket-spot-vm:/dev# ls
autofs           hugepages           null    shm       tty14  tty27  tty4   tty52  tty8     vcsa   vfio
block            hwrng               psaux   snapshot  tty15  tty28  tty40  tty53  tty9     vcsa1  vga_arbiter
bsg              initctl             ptmx    stderr    tty16  tty29  tty41  tty54  ttyS0    vcsa2  vhost-net
btrfs-control    input               pts     stdin     tty17  tty3   tty42  tty55  ttyS1    vcsa3  vhost-vsock
char             kmsg                random  stdout    tty18  tty30  tty43  tty56  ttyS2    vcsa4  zero
console          log                 rtc     tpm0      tty19  tty31  tty44  tty57  ttyS3    vcsa5
core             loop-control        rtc0    tpmrm0    tty2   tty32  tty45  tty58  urandom  vcsa6
cpu_dma_latency  mapper              sda     tty       tty20  tty33  tty46  tty59  vcs      vcsu
cuse             mem                 sda1    tty0      tty21  tty34  tty47  tty6   vcs1     vcsu1
disk             memory_bandwidth    sda14   tty1      tty22  tty35  tty48  tty60  vcs2     vcsu2
fd               mqueue              sda15   tty10     tty23  tty36  tty49  tty61  vcs3     vcsu3
full             net                 sdb     tty11     tty24  tty37  tty5   tty62  vcs4     vcsu4
fuse             network_latency     sg0     tty12     tty25  tty38  tty50  tty63  vcs5     vcsu5
hpet             network_throughput  sg1     tty13     tty26  tty39  tty51  tty7   vcs6     vcsu6

```



It's a character device based file Within Linux devices such as hardware are characterised in two ways:

Character Devices (c) which are devices which transfer data in characters also known as bytes or bits such as mice, speaker etc.

Block Devices (b) which are devices which transfer data in blocks of data such as USB, Hard Disks etc.


![image](https://user-images.githubusercontent.com/38061560/154807795-2e66a94c-43f3-44b9-b865-4e43142f9968.png)

- what is tty?

The tty command of terminal basically prints the file name of the terminal connected to standard input. tty is short of teletype, but popularly known as a terminal it allows you to interact with the system by passing on the data (you input) to the system, and displaying the output produced by the system.

![image](https://user-images.githubusercontent.com/38061560/154807841-0dcca983-07b5-462e-b054-592f18dfb828.png)

it shows /dev/pts/0

if you open another session then the output will be changed .

![image](https://user-images.githubusercontent.com/38061560/154808150-6e2086e9-f56b-4a42-96c7-82314273d9be.png)


as you can see  /dev/pts/0  and /dev/pts/1 . this are the terminal attached to our process -> ps -a 
 
- what is stty?

stty command in Linux is used to change and print terminal line settings

`stty size`

it gives size of terminal [ length X Breath ]

![image](https://user-images.githubusercontent.com/38061560/154807983-0b354461-7979-45cc-bbba-87bedae6a948.png)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------
5. /etc 

This Directory Contains all of the system-wide Configuration Files.

It also contains a collection of shell scripts that start each of the system services at boot time.

Everything in this directory should be readable text.

some Interesting Files:

- /etc/fstab   : It contains the details about storage devices and thier associated mount points.

```
UUID=6e8u8db3-b63e-4603-9fd7-fb7ada8908cd / ext4 rw,discard,errors=remount-ro,x-systemd.growfs 0 1  --for Boot disk
/dev/sdb /data ext4 defaults 0 1  --for non boot disk


```
- /etc/passwd  : It contains a list of the user accounts. The syntax is as follows
``` 
sanket_bisne:x:1001:1002:sanket_bisne,1,1,1,1:/home/sanket_bisne:/bin/bash
```
- /etc/crontab : It contains a file that defines when automated jobs will be Run.
```
SHELL=/bin/sh
PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin

# Example of job definition:
# .---------------- minute (0 - 59)
# |  .------------- hour (0 - 23)
# |  |  .---------- day of month (1 - 31)
# |  |  |  .------- month (1 - 12) OR jan,feb,mar,apr ...
# |  |  |  |  .---- day of week (0 - 6) (Sunday=0 or 7) OR sun,mon,tue,wed,thu,fri,sat
# |  |  |  |  |
# *  *  *  *  * user-name command to be executed
17 *    * * *   root    cd / && run-parts --report /etc/cron.hourly
25 6    * * *   root    test -x /usr/sbin/anacron || ( cd / && run-parts --report /etc/cron.daily )
47 6    * * 7   root    test -x /usr/sbin/anacron || ( cd / && run-parts --report /etc/cron.weekly )
52 6    1 * *   root    test -x /usr/sbin/anacron || ( cd / && run-parts --report /etc/cron.monthly )
#

```
- /etc/sudoers : 

Within your Linux or macOS system, there’s a file called “sudoers” which controls the deepest levels of your permissions system. It permits or denies users from gaining super-user access and holds some special preferences for sudo.

- What is the sudoers file?
The sudoers file is a text file that lives at "/etc/sudoers." It controls how sudo works on your machine. 
This permits your users to execute commands that would be otherwise prohibited.

If you need to grant it superuser permission, you will need to edit the sudoers file and add this user account to it.

The main purpose of the sudoers file is to control which users can run sudo. Without sudo, users can’t elevate their permissions. If you have multiple users accessing the same system through shells, you can control their access by setting values in sudo.

Every sudoers file will have the following line:

`root ALL=(ALL) ALL`
This permits the root user on ALL hosts using ALL users to execute ALL commands. ALL is a special value in the sudoers file meaning "no restrictions."

To Add new user to your sudoers file then follow the steps:

- `adduser sanket_bisne` 
- nano /etc/sudoers
- sanket_bisne ALL=(ALL) ALL
- ctrl o , ctrl x
- sudo su - sanket_bisne
- enter password
- run apt update and now you have all privileges.

and other files like os-release etc are present in the etc directory.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------


