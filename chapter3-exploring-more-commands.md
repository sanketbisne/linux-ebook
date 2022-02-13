<h2> Exploring more Commands with their flags </h2>

1.  ls

As we saw earlier ls command is used to list down files/Folder in Directories
if we want some hidden files ie which start with . in linux
to be displayed on the terminal we can use 

 Normal ls 

![image](https://user-images.githubusercontent.com/38061560/153747237-849dfa45-ee58-4769-95f6-c79f521f9d91.png)

- ls -a  ->  It list all files and also which starts from . (hidden files).
- ls -l  -> display result in long list
- ls -al ->  It displays results in long format.

![image](https://user-images.githubusercontent.com/38061560/153747227-1b99b4f8-9a92-479c-9604-41240a53003a.png)

- ls -F  -> It appends an indicator charactor to the end of each listed name. / if the name is directory.

![image](https://user-images.githubusercontent.com/38061560/153747282-39b6cdb9-ddfb-4d88-aff5-480ea5382f85.png)

- ls -r  -> Displays results in reverse order

![image](https://user-images.githubusercontent.com/38061560/153747301-879a41d5-ba2d-450d-a5c7-2823ad2c5f45.png)

- ls -t  -> Sorts by modification time

![image](https://user-images.githubusercontent.com/38061560/153747317-404e97da-bffd-4be7-bc8f-903c1d72fbb1.png)

- ls -s  -> sorts output by file size

![image](https://user-images.githubusercontent.com/38061560/153747329-5787cc11-6f7d-40ec-9586-5368e0c0fc56.png)

- ls -ltrh -> print the output in long listed , sorted by modification time  and human readable format.

![image](https://user-images.githubusercontent.com/38061560/153747348-a7695a17-666c-4a27-97e6-faaf1ac1fcec.png)

<h3> About File Permission user , owner and groups </h3>

what does first column `-rw-r--r--` means ?

The first character tells the
type of file. Among the different types, a leading dash(-)
means a regular file, while a "d" indicates a directory.
Lets split down this into 3 units.

`-` means that it is file
`d` means that it is a directory

`rw-` means that there is read and write permission granted on Owner level
`r--` means that there is only read permission granted on group 
`r--` means that there is onlt read permission granted for everyone else ie. others

`root` - The username  of the file's owner
`root` - The name of the group that owns the file.
`