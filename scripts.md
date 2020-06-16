In this document, I am trying to explain some of scripts for taking easy and getting you faster on terminal and nautilus

### Scripts on terminal
| Type | Command |
|-|-|-|
|Copy clipboard|`'alias cpwd="pwd | tr -d '\n' | pbcopy && echo 'pwd copied to clipboard'`|
|Find text in path's folder|`'alias ftext="grep -rnw $1 -e '$2'"`|

> **Note:** You should add to **~/.bashrc** file that described all of scripts above

### Open terminal shortcut on nautilus

This is common problem for mouse hater people. If you wonder to do it follow the below steps.

- Add a file named `Terminal` which is located `~/.local/share/nautilus/` and edit with terminal app which is you are using.
	```sh
	#!/bin/bash
	terminator
	```
-  Then make the `Terminal` file to executable and quit from all nautilus
	```sh
	chmod +x Terminal
	nautilus -q
	```
- Then navigate to `~/.config/nautilus/scripts-accels` file. If it is not existed located area, you should create the file and add below the script to `scripts-accels` which shortcut you would like to use. In here I choose `F12` button
	 ```sh
	 F12 Terminal
	 ```
- Now it will work ! If you want to check right click on nautilus, you will see the your script at there.
	 
