<h2> Intro to FileSystem </h2>

-  What Is the FileSystem?

Like Windows, a Unix-like operating system such as Linux organizes its files in what is
called a hierarchical directory structure. This means they are organized in a tree-like pat-
tern of directories (sometimes called folders in other systems), which may contain files
and other directories. The first directory in the file system is called the root directory. The
root directory contains files and subdirectories, which contain more files and subdirecto-
ries and so on.

Note that unlike Windows, which has a separate file system tree for each storage device,
Unix-like systems such as Linux always have a single file system tree, regardless of how
many drives or storage devices are attached to the computer. Storage devices are attached
(or more correctly, mounted) at various points on the tree according to the whims of the
system administrator, the person (or people) responsible for the maintenance of the sys-
tem.

For Navigation File System we use basically 3 Commands

- cd
change directory

- pwd 
present working directory

- ls 
list Directory

![image](https://user-images.githubusercontent.com/38061560/153715847-14602cb1-3962-4975-bccf-f5318cef1cfb.png)


- File System hierarchy

Here in Linux , Files are organized in a tree like pattern of directories.

So the First Directory is the `Root` Directory which contains files and other Directories.

Under Root there are many Directories and Sub-Directories under it .

- Absolute and Relative Pathnames 

Absolute Path begins with the root directory and ends untill the desired directory or file is completed.

For example : there is a directory on our system in which most of oour system's programs are installed.

PathName is `/usr/bin`  the / is root directory and /usr contains directory called /bin.

![image](https://user-images.githubusercontent.com/38061560/153716265-e9928784-05c6-4b80-a9dd-f4c551f07e0c.png)

now we will navigate to directory "sample" using absolute path
cd /usr/bin/sample

![image](https://user-images.githubusercontent.com/38061560/153716365-fb90322c-754e-424b-85b8-343ba48c8a2a.png)

Relative Pathnames starts from working directory .
Using . and ..
cd ./bin/sample

![image](https://user-images.githubusercontent.com/38061560/153716695-a3353041-1ab3-468a-b036-66c0734f75e9.png)

.. is used to go back to the parent directory or one step behind 
we are going back from sample to root one by one using `cd ..`
![image](https://user-images.githubusercontent.com/38061560/153716944-af9b1496-6e08-478c-8ab9-9f459736350c.png)

"cd -"  is used to go back to the previous working directory

![image](https://user-images.githubusercontent.com/38061560/153717062-d27ffb31-2fec-4dfb-b5ba-fc5f38f97163.png)
 as we can see we were previously on the directory /bin/usr and now we navigated to /var/www/html
so when we enter command `cd -` we are navigated back to the /bin/usr ie the previous directory.

![image](https://user-images.githubusercontent.com/38061560/153717104-11ca3653-5dae-4269-af36-6aa5af9dc904.png)
