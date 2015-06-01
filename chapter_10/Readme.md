##Chapter 10 Readme

>What is Robocopy?

Robocopy is a copy command for use in the Windows OS command line.  It means "Robust File Copy" which is different from <br/>
normal copy in a few ways.  For one, it is more reliable at copying or mirroring large files or directories that the <br/>
standard Windows `xcopy` and it also has a built in "resume copy" feature in case that a copy procedure gets interrupted<br/>
Robocopy also allows every aspect of a file to be copied, including time-stamps, attributes, and security properties.


##Do More

>Use the cp -r command to copy more directories with files in them.

To do this I first made a new directory with two empty files in it: `mkdir mas_dir` ; `touch empty.md also_empty.md` <br/>
I then copied the whole diretory and its contents using the `cp -r` command: <br/>
`cp -r mas_dir other` => this made a copy of the 'mas_dir' contents and put them in the new dirctory 'other'<br/>
To see that this worked I used `ls other`, which returned `also_empty.md empty.md`

>Copy a file to your home directory or desktop.

Lets assume that I'm still in the 'chapter_10/tmp' directory.  I'll copy the file 'also_empty.md' to my home directory<br/>
by typing: `cp other/also_empty.md ~/`

I then check that that actually copied the file to where I wanted => `ls ~/`, and sure enough, 'also_empty.md' is there

>Find these files in your graphical user interface and open them in a text editor.

In my finder I'll click through the folders: workspace, davinci_coders_t2_2015, homework, learn_command_line_exercises, <br/>
chapter_10, and finally into the tmp folder.  Once there I double click on awesome.txt to open in up in my text editor. <br/>
It doesn't have anything in it -- empty.

*Notice how sometimes I put a / (slash) at the end of a directory? That makes sure the file is really a directory, <br/>
so if the directory doesn't exist I'll get an error.*


###Alternative "english" ways of asking you to copy a file:

>Can you copy the foo.txt file to slash temp?  (Create foo.txt first...)

You can indeed!  First create 'foo.txt' with `touch foo.txt` <br/>
Then to copy that file to the temp directory just type: `cp foo.txt /tmp/`<br/>
And viola! the foo.txt file has been copied to the tmp directory. <br/>
You can check this by calling `ls /tmp` and look for the foo.txt file

>Can you copy .bash_profile in your home directory to the current directory?

if you type: `cp ~/.bash_profile ./` in the terminal, a copy of the '.bash_profile' will be made <br/>
in your current working directory.

You can check this by simply calling `ls -a` and seeing if the .bash_profile file is in fact there.
