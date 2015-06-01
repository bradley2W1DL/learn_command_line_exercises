##Chapter 16 readme

**Alternative "english" ways of asking for your working directory:**

>Can you show me all the files in slash temp slash foo?

`find /tmp/foo/ -name "*" -print` Will print out all the file names within the '/tmp/foo' directory

>What log files are in your log directory?

`find /log/ -name "*.log" -print` will print out all the log files that're in the log directory.

___

*Run a find in the class directory, pipe the output to pbcopy, and create a gist with the content*

https://gist.github.com/bradley2W1DL/89fbe18f35c82d6de072
