#Chapter 6
<br/>
>What does the command `ls -lR` show us?

The `ls -lR` command shows us all of the files and directories within a directory in the long listing format recursively. <br/>
The 'recursively' part mean that the `ls -l` command is then repeated in each directory within the parent directory, thereby <br/>
displaying the long listing format for each file within all subsequent child directories.

<br/>
Alternative "english" ways of asking for a list of files:<br/>

>What's in the tmp directory?

lets find out; type: `ls tmp` <br/>
my terminal output:<br/>
`iamcool.txt` *naturally* <br/>
and it should be noted that my `pwd` here is: ~/workspace/davinci_coders_t2_2015/homework/learn_command_line_exercises

>Can you show me what files are in that directory?

sure thing: `ls "that directory"` will list for you all the files in 'that directory'.

>What files are in your home directory?

type: `ls ~` <br/>
this displays all the files and directories within my home directory...<br/>
![alt text](https://github.com/bradley2W1DL/learn_command_line_exercises/blob/master/pics/1__bash_ls~.png "bash for ls ~")

>What's in slash temp?

The command to run in order to find that out is: `ls /tmp` <br/>
this lists everything in the /tmp directory; which for me is... <br/>
![alt text](https://github.com/bradley2W1DL/learn_command_line_exercises/blob/master/pics/bash_ls_slash-tmp.png "bash for ls /tmp")

###Comments

I do have a question regarding the specifics of what is displayed in the 'long listing format' <br/>
For example, if I call `ls -l ~/workspace/` the terminal returns: <br/>
total 0 <br/>
drwxr-xr-x@  6 bird  staff  204 May 18 22:44 DaVinci Videos <br/>
drwxr-xr-x@ 10 bird  staff  340 May 18 20:56 davinci_coders_t2_2015 <br/>
drwxr-xr-x  11 bird  staff  374 May 16 13:32 pivotal_ide_prefs <br/>
I'm not sure what the `drwxr-xr-x@  6 bird  staff  204` means -- so I guess I'll look into that: <br/>
<br/>
