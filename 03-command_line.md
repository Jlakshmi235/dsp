# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > My cheat sheet
>>1. show current working directory path  - **`pwd`**
>>2. creating a directory - **`mkdir <dirname>`**
>>3. deleting a directory - **`rm -rf <dirname>`**
>>4. creating a file using `touch` command - **`touch <filename>`**
>>5. deleting a file - **`rm <filename>`**
>>6. renaming a file - **`mv <cur filename> <new filename>`**
>>7. listing hidden files - **`ls -a`**
>>8. copying a file from one directory to another - **`cp <filename> <dirname>`**
>>9. changing directory - **`cd <sub dirname>`** or **`cd <path to directory>`**
>>10. go to parent directory - **`cd ..`**
>>11. displaying contents of a file - **`cat <filename>`** or **`less <filename>`** or **`more <filename>`**
>>12. displaying the number of lines, words, and characters in a file - **`wc <filename`**
---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

>> `ls` - lists all visible directories and files present  
>>`ls -a` -  lists hidden files along with visible directories and files
>>`ls -l` -  displays the long format listing 
>>`ls -lh` - displays the size in bytes  
>>`ls -lah` - displays the long format listing of hidden files also 
>>`ls -t` - lists directories and files sorted according to timestamp (newest first)  
>>`ls -Glp` - displays the long format listing and directories end with **/**  

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

>>1. **`-R`** - displays subdirectories as well
>>2. **`-m`** - displays content in csv format
>>3. **`-d`** - displays only directories
>>4. **`-t`** - lists directories and files sorted according to timestamp (newest first) 
>>5. **`-u`** - displays files by file access time

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > `xargs` has the ability to apply a given command to a series of items piped through in order. The default command is echo.
Example: suppose we want to find all pdf files in a directory and convert them to text files. We can use the following statement.
```console
find . -name '*.pdf' | xargs -n1 pdftotext
```


 

