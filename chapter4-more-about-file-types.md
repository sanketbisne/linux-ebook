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


