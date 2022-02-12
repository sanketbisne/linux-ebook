<h2> Intro to FileSystem </h2>

-  What Is the FileSystem?

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



