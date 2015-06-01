##Chapter_15

*Alternative "english" ways of asking for pipes and redirection:*

>Can you put "This class is fun" into bar.txt?

yes I can: `echo "This class is fun" > bar.txt` *This writes "This class if fun" to 'bar.txt', and overwrites anything* <br/>
*that was in there previously*

>Can you put "Oh so much fun" into foo.txt?

type: `echo "Oh so much fun" >> foo.txt` *this appends 'foo.txt', adding that statement on another line below any* <br/>
*existing text that's already in foo.txt*

**The following symbols were used in this chapter.  Here's a breakdown of their function**

**|** -- the pipe, will 'pipe' the output of the command to the left of the symbol to the command on the right.

  for example, `cat  ex13.txt ex12.txt ex14.txt | less` would take the output of all three ex*.txt files listed and <br/>
  pass their output to the `less` command.  In effect this combines the contents of all three .txt files and passes it<br/>
  to the `less` file viewer.

< the less-than symbol will pass the input from the right side of the symbol to the command on the left.

'>' greater than -- gives the output from the command/file on the left to the file on the right.

'>>' double greater-than -- appends the file on the right with the output of command/file on the left
  <br/>E.g. `echo 'this is cool' >> ex12.txt` will add the line 'this is cool' to the ex12.txt file, but it will not <br/>
  overwrite the previous contents (as the '>' would)
