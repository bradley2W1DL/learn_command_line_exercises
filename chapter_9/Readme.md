##Chapter 9 Readme

####Unix: Do More Question

>Unix: Make a directory, change to it, and then make a file in it. Then change one level up and run the rmdir command in this directory.<br/>
You should get an error. Try to understand why you got this error.

I put the file `fizzle.txt` inside the tmp directory then backed out of it and tried to `rmdir tmp` <br/>
This gives you the error: `rmdir: tmp: Directory not empty`<br/>
Meaning that you can't delete a directory that has any files or other directories in it using just the `rmdir` command.

####Alternative "english" ways of asking you to create a file:

>Can you touch blah.txt?

That I can: typing `touch blah.txt` will create the empty text file 'blah' in the current working directory.

>Let's create foo.txt.

Okeedoke: `$ touch foo.txt`

>What happens if you touch an existing file?

touching an existing file will change the time of last modification on that file.  This can be viewed with the <br/>
long listing format of that file.

For example:
![alt text](https://github.com/bradley2W1DL/learn_command_line_exercises/blob/master/pics/touch_timeUpdate.png "touch time update")

Here I first looked at a file that was created about a week ago (`ls -l README.md`) in the -l format so that it would<br/>
show the date that the file was last modified.

I then called `touch` on the file and again checked its long listing.  And sure enough the date of last modification was<br/>
changed to the time at which the `touch` command was called even though the contents of the file wasn't changed, nor <br/>
was the file even opened.
