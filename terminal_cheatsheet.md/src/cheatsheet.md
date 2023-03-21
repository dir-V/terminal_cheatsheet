# Terminal Cheatsheet

### Navigation: <br>
* `cd` (change directory) - allows for navigation to a folder within the current directory <br>
```
➜  week_01 cd day_1
➜  day_1 
```
> Using `..` after `cd` will return to the parent folder.
```
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
``` 
➜  day_1 pwd
/Users/vincent/bnta_work/week_01/day_1
```
<br />
<br />


### Creating and Deleting Files:
* `mkdir` - creates new folder
>Note: Adding a space in the name of a folder/file will create two different folders/files.

<br />

* `touch` - creates new file


>Note: This will be highlighted

`Make text appear differently`

If you want to emphasize something you can use backtick ```

```` java
public boolean isEnough(){
    return true;
   }
````