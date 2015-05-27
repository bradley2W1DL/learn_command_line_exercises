##Chapter 5 readme
*As you'll learn in this chapter, cd (change directory) allows you to change your present working directory.* <br/>

Note that Linux/OSX uses /, while Windows uses . In "english" I will simply say slash, you should remember which slash you should use.<br/>
**Alternative "english" ways of asking you to change directories:**
<br/><br/>
>Can you cd into the temp directory?

certainly: `cd ~/workspace/davinci_coders_t2_2015/homework/learn_command_line_exercises/chapter_5/temp`

>Please go into the temp directory?

depending upon where you are currently you would type: `cd tmp`

>Can you go to the slash temp directory?

yes: `cd /tmp` 

>Can you go to the slash temp slash log directory?

yea: `cd /tmp/log` *though, on my computer this this directory doesn't appear to exist.  the `log` part at least*

>What does the .. argument to cd do?

The `..` argument tells the cd command to back out of the current directory to its parent directory.<br/>
In other words, if your `pwd` is ~/workspace/stuff/things and you pass `cd ..` you will be moved to <br/>
back to the ~/workspace/stuff directory.



##Do More Section

> cd to the joe directory with one command.

Assuming that you're in the `pwd`: /Users/bird/workspace/davinci_coders_t2_2015/homework/learn_command_line_exercises <br/>
You would type: `cd chapter_4/temp/stuff/things/frank/joe/`

> cd back to temp with one command, but not further above that.

type: `cd ../../../../` This should get you back to temp; double check with `pwd`

> Find out how to cd to your "home directory" with one command.

type: `cd ~` to get back to home directory. *Or the command `cd` on it's own will return you to the home directory*

> cd to your Documents directory, then find it with your GUI file browser (Finder, Windows Explorer, etc.).

1. in terminal: `cd ~/Documents`
2. In GUI: click on Finder, then 'home directory' in left sidebar, and then click on the Documents folder

> cd to your Downloads directory, then find it with your file browser.

1. in terminal: `cd ~/Downloads`
2. in GUI: open the Finder and click on Downloads folder in the sidebar.

> Find another directory with your file browser, then cd to it.

* In the GUI I navigated to the 'Steel' folder in my Google Drive <br/>
to access that in the command line I type: `cd ~/"Google Drive"/Steel`

