# linux-ebook
This Ebook gives you basic knowledge about Linux . 

<h2> Intro to Shell </h2>

-  What Is the Shell?

The shell is a program that takes keyboard commands and passes them to the operating system to carry
out. Almost all Linux distributions supply a shell program from the GNU Project called
bash.

The name "bash" is an acronym for “Bourne Again SHell”, a reference to the fact
bash is an enhanced replacement for sh, the original Unix shell program written by
Steve Bourne.

- Terminal Emulators

When using a graphical user interface (GUI), we need another program called a "terminal
emulator" to interact with the shell.

KDE uses konsole and GNOME uses gnome-terminal, though it's
likely called simply “terminal” on our menu.

- Launching Terminal

If you are using ubuntu just type "ctrl + alt + t " it will open the new terminal.

- So Basically What is $ ?

![shell-prompt](https://user-images.githubusercontent.com/38061560/152686576-9b4f8de4-6def-41d2-957d-93730f0ec339.png)

$ is a shell prompt and it will appear on the terminal, whenever the shell is ready to accept input.

![image](https://user-images.githubusercontent.com/38061560/152687226-66c86048-cfea-406c-857e-e7d16b1f4e79.png)

If the last character of the prompt is a pound sign (“#”) rather than a dollar
sign, the terminal session has superuser privileges. 
ie sudo su .

This means either we are
logged in as the root user or we selected a terminal emulator that provides superuser (administrative) privileges.

Some Simple Commands
`date` - displays the current time and date.
![image](https://user-images.githubusercontent.com/38061560/152687564-6b93d5e5-7987-415b-b906-0acff41fc263.png)

`cal`  - to display calender
![image](https://user-images.githubusercontent.com/38061560/152687587-1cf6e2c6-6338-49e6-9646-48a3587f4ac6.png)

`df` -  To see the current amount of free space on our disk drives, enter df. and if you want in human readable form then type 
` df -h `

![image](https://user-images.githubusercontent.com/38061560/152687685-f83ad253-15f0-4fc4-87a5-899f337c0377.png)

`free` - Likewise, to display the amount of free memory, enter the free command.
![image](https://user-images.githubusercontent.com/38061560/152687740-2961542e-7d4b-48e8-b439-30e838a2a339.png)

`exit` - We can end a terminal session by either closing the terminal emulator window, by entering the exit command at the shell prompt, or pressing Ctrl-d.

![image](https://user-images.githubusercontent.com/38061560/152687807-b63a32db-d326-4cce-a986-fcfa25f49f75.png)

This is all about the introduction to Shell










