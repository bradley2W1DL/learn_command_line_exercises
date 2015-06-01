##Chapter 21 Readme.md

###Do More
___

I want you to go online and research how you change your PATH for your computer. Try to do it entirely from the CLI.

So the PATH is an environment variable in your environment that contains a list of directories, separated by a colon, <br/>
that your shell searches through when you enter a command.  Program files (executables) that are called with commands <br/>
are stored in different places on your machine and your PATH tells the Unix shell where to look for them.<br/>
In this list, earlier entries in the list will take precedence over later ones.

The PATH on my computer is: <br/>
![alt text](https://github.com/bradley2W1DL/learn_command_line_exercises/blob/master/pics/%24PATH.png "$PATH")

You can append new directories onto the end of your path by typing: <br/>
`PATH = $PATH\:/new_directory/path ; export PATH`

Or, if you want the path you designate to come first in $PATH you can enter to command this way: <br/>
`PATH = /new_directory/path:$PATH ; export PATH`

###Alternative "english" ways of asking for your working directory:
___

You can find the answer to the following three questions by typing `env` into the terminal and looking at the output...

>What is your shell set to?

My shell is set to: `SHELL=/bin/bash`

>What directory are you in (don't use pwd this time)?

my pwd (as shown in my environment listing) is: <br/>
`PWD=/Users/bird/workspace/davinci_coders_t2_2015/homework/learn_command_line_exercises/chapter_21`

>What is your home directory set to?

My home directory is set to: `HOME=/Users/bird`

>Can you set your environment to have DEBUG set to true?

Yes I can: `export DEBUG=true` will set a new environment variable, DEBUG, to true.<br/>
you can check to see if this happened by either: 

1. typing `env` and looking through until you find DEBUG
2. typing: `echo $DEBUG`. This will return the value assigned to $DEBUG, i.e. 'true'.
3. Or you can search in the `env` with `env | grep DEBUG`, which will return DEBUG=true
