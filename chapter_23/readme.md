##Chapter 23 readme
___

`$ exit` => this exits you out of your current shell.
___

**Alternative "english" ways of asking for your working directory:**

>Let's close this terminal and open a new one.

`exit` will close your terminal window, and then you have to use the GUI and select 'New Window' from the 'Shell' <br/>
menu on the top bar.  Or you can use the keyboard shortcut 'command N'

>Can you reload your terminal?

In iTerm you can use the keyboard shortcut 'command R' to restart your terminal.  or you can use the command `exit` to <br/>
close out of your shell and then open up a new one.

>Can you logout?

the command `logout` seems to have the same effect as `exit`, in that it closes your shell window.<br/>
You can also use the `login` command to change users.  After typing in login it will prompt you for a username <br/>
and password and then return the last time that user was logged in.
___

**Do More**

Explain the following commands:

1. xargs => The xargs command can take a list of strings and pass them to another command as arguments.  It works as <br/>
a sort of loop that allows you to run the same command on a list of different inputs all at once.
2. sudo => Allows the user to execute a command as the superuser or as another user.  Using this command requires <br/>
permissions and will prompt the user for a password.  It will be their user password if they have been given permission <br/>
to use `sudo` in the config file `/etc/sudoers`
3. chmod => 'Change permissions modifiers' -- this command allows to file owner or superuser to change file modes or <br/>
control access on a file. Permissions can be set to allow **Read, Write, eXecute**, or any variation of the three <br/>
for the three main user groups -- owner, group (that a file or dir belongs to), and any other user.<br/>
*I wrote about this in a bit more detail at [my blog](https://bradleyberger.wordpress.com/2015/05/25/understanding-long-listing-format-in-unix/)*
4. chown => allows you to change the file owner ID and/or the group ID on specified files.  The ownership of a file <br/>
can only be changed by a super-user and the group ID can only be changed by a member of that group.
