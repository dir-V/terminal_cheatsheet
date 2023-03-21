# Terminal Cheatsheet

### Navigation: <br>
* `clear` clears current 
* `cd` (change directory) - allows for navigation to a folder within the current directory <br>
``` shell
➜  week_01 cd day_1
➜  day_1 
```
> Using `..` after `cd` will return to the parent folder.
```shell
➜  day_1 cd ..
➜  week_01 
```

> Using `cd` with no argument will return to the root directory.
```shell
➜  day_1 cd
➜  ~ 
```
<br />

* `pwd` - (print working directory) - Shows the path to the current folder you are in.
```shell
➜  day_1 pwd
/Users/vincent/bnta_work/week_01/day_1
```
<br />

* `ls` - Lists all files and folders in the current directory.
```shell
➜  ~ ls
Desktop     Downloads   Movies      Pictures    Public      test_folder
Documents   Library     Music       Postman     bnta_work
➜  ~ 
```
> The `ls` command can also take certain arguments. Adding `-l` shows additional information about folders and files. Adding `-a` shows hidden folders and files withing the directory.
```shell
➜  ~ ls -l 
total 0
drwx------+  5 vincent  staff   160 21 Mar 16:11 Desktop
drwx------+  4 vincent  staff   128 21 Mar 11:09 Documents
drwx------+  7 vincent  staff   224 20 Mar 13:44 Downloads
drwx------@ 84 vincent  staff  2688 20 Mar 22:36 Library
drwx------   4 vincent  staff   128 17 Mar 15:15 Movies
drwx------+  4 vincent  staff   128 20 Mar 11:54 Music
drwx------+  4 vincent  staff   128 16 Mar 09:39 Pictures
drwxr-xr-x   3 vincent  staff    96 17 Mar 14:05 Postman
drwxr-xr-x+  4 vincent  staff   128 16 Mar 09:17 Public
drwxr-xr-x  16 vincent  staff   512 21 Mar 11:23 bnta_work
drwxr-xr-x   2 vincent  staff    64 21 Mar 16:15 test_folder
➜  ~ 
```
```shell
➜  ~ ls -a
.
..
.CFUserTextEncoding
.DS_Store
.Trash
.android
.gitconfig
.lesshst
.m2
.oh-my-zsh
.ssh
.vscode
.zcompdump-Vincent’s MacBook Air-5.8.1
.zprofile
.zsh_history
.zsh_sessions
.zshrc
Desktop
Documents
Downloads
Library
Movies
Music
Pictures
Postman
Public
bnta_work
test_folder
➜  ~ 
```
> Both the `-l` and `-a` command can be used together to show hidden folders and additional information.
```shell
➜  ~ ls -la
total 168
drwxr-x---+ 28 vincent  staff    896 21 Mar 16:50 .
drwxr-xr-x   5 root     admin    160 16 Mar 09:17 ..
-rw-------   1 vincent  staff      3 16 Mar 09:17 .CFUserTextEncoding
-rw-r--r--@  1 vincent  staff  10244 21 Mar 12:41 .DS_Store
drwx------+  5 vincent  staff    160 21 Mar 16:11 .Trash
drwxr-xr-x   2 vincent  staff     64 21 Mar 14:55 .android
-rw-r--r--   1 vincent  staff    122 21 Mar 13:55 .gitconfig
-rw-------   1 vincent  staff     20 21 Mar 14:03 .lesshst
drwxr-xr-x   3 vincent  staff     96 21 Mar 15:00 .m2
drwxr-xr-x  23 vincent  staff    736 20 Mar 14:38 .oh-my-zsh
drwx------   6 vincent  staff    192 21 Mar 11:38 .ssh
drwxr-xr-x   4 vincent  staff    128 17 Mar 12:47 .vscode
-rw-r--r--   1 vincent  staff  48121 20 Mar 14:38 .zcompdump-Vincent’s MacBook Air-5.8.1
-rw-r--r--   1 vincent  staff     85 17 Mar 13:39 .zprofile
-rw-------   1 vincent  staff   5671 21 Mar 16:50 .zsh_history
drwx------  20 vincent  staff    640 21 Mar 10:06 .zsh_sessions
-rw-r--r--   1 vincent  staff   3866 20 Mar 14:38 .zshrc
drwx------+  5 vincent  staff    160 21 Mar 16:11 Desktop
drwx------+  4 vincent  staff    128 21 Mar 11:09 Documents
drwx------+  7 vincent  staff    224 20 Mar 13:44 Downloads
drwx------@ 84 vincent  staff   2688 20 Mar 22:36 Library
drwx------   4 vincent  staff    128 17 Mar 15:15 Movies
drwx------+  4 vincent  staff    128 20 Mar 11:54 Music
drwx------+  4 vincent  staff    128 16 Mar 09:39 Pictures
drwxr-xr-x   3 vincent  staff     96 17 Mar 14:05 Postman
drwxr-xr-x+  4 vincent  staff    128 16 Mar 09:17 Public
drwxr-xr-x  16 vincent  staff    512 21 Mar 11:23 bnta_work
drwxr-xr-x   2 vincent  staff     64 21 Mar 16:15 test_folder
```
<br />
<br />

### Creating and Deleting Files:
* `mkdir` - creates new folder
>Adding a space in the name of a folder/file will create two different folders/files.

<br />

* `touch` - creates new file
> Always specify the extension of the file you want to create. Example: touch example.txt

<br />

* `rm` - completely deletes a file
> To delete a folder using the `rm` command `-r` argument needs to added to command.

<br />
<br />

### Manipulating Files and Folders:
* `open` - allows a file to be opened

<br />

* `cp` - copies a  file
> By default, executing this command alone will try to copy the file in the same directory as you are in with the exact same name, leading to an error. The location of where you want to copy the file to must also be added.

<br />

* `mv` - allow for files to be moved to a different folder

<br />
<br />

### Git Commands:
* `git init` - initialises a git repository in the current directory you are in
* `git_status` - shows the current status of the git repository
* `git add` - adds a change in the working directory to the staging area
* `git commit` - uploads a snapshot of the changes added to the files
* `git push` - pushes a local file/folder to the cloud git repository.
* `git ignore` - adds a `ingore` rule to certain files so that they are not pushed to the remote repository.
