#Chapter 6
<br/>
>What does the command `ls -lR` show us?

The `ls -lR` command shows us all of the files and directories within a directory in the long listing format recursively. <br/>
The 'recursively' part mean that the `ls -l` command is then repeated in each directory within the parent directory, thereby <br/>
displaying the long listing format for each file within all subsequent child directories.

<br/>
Alternative "english" ways of asking for a list of files:<br/>

>What's in the tmp directory?

lets find out; type: `ls /tmp` <br/>
my terminal output:<br/>
`KSOutOfProcessFetcher.501.IW-ShwaXJwmHlkfc5wb2ZMHOaJY=
amt3.log` <br/>
`com.apple.launchd.25YhkaRfVt` <br/>
`com.apple.launchd.suB1oFhnNm` <br/>
`swtag.log`

>Can you show me what files are in that directory?
>What files are in your home directory?

but of course: `ls ~` <br/>
this displays all the files and directories within my home directory...<br/>
![alt text](https://github.com/bradley2W1DL/learn_command_line_exercises/blob/master/pics/1__bash_ls~.png "bash for ls ~")


>What's in slash temp?

###Comments

I do have a question regarding the specifics of what is displayed in the 'long listing format' <br/>
For example, if I call `ls -l ~/workspace/` the terminal returns: <br/>
total 0 <br/>
drwxr-xr-x@  6 bird  staff  204 May 18 22:44 DaVinci Videos <br/>
drwxr-xr-x@ 10 bird  staff  340 May 18 20:56 davinci_coders_t2_2015 <br/>
drwxr-xr-x  11 bird  staff  374 May 16 13:32 pivotal_ide_prefs <br/>
I'm not sure what the `drwxr-xr-x@  6 bird  staff  204` means -- so I guess I'll look into that: <br/>
<br/>
