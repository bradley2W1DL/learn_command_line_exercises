##Chapter 19 Readme

*Alternative "english" ways of asking for your working directory:*

>What option to ls tells it to output file size in human readable form?

I don't know, but we can find out by typing `man ls` into the terminal.<br/>
      - So, when when the '-h' option is used with the '-l' (long listing format) option it will make the file sizes <br/>
      more readable by using unit suffixes; such as Byte, Kilobyte, Mega, Giga, Tera, and Petabyte rather than just <br/>
      listing file sizes in bytes.

>Is there a case insensitive option to grep?

that there is, the '-i' option will tell grep to perform its search to return matches even if the cases don't match <br/>
the search query.

>What does the -r and -f options to rm do exactly?

hmmmm: `man rm`...<br/>

So, the -f option tells the rm command to remove files without prompting you for confirmation, regardless of the <br/>
permissions. (Which can make that a fairly dangerous command)<br/>
And the -r option tells the `rm` command to run again in each subsequent directory within the directory in which you <br/>
called the `rm` in initially.  In other words, recursively.

>What does the ifconfig command do?

`man ifconfig` => The `ifconfig` command is a utility that allows you to assign an address to a network interface <br/>
 and/or configure network interface parameters.

