## Chapter 12 readme

Alternative "english" ways of asking for your working directory:<br/>

>Can we see what's in our production log?

yes, just type: `more production.log` or if the file is really large: `less production.log` and then navigate through <br/>
the file with 'space', 'w', arrow keys, or whatever.

>What does our database.yml look like?

`more database.yml` <br/>
`less database.yml` => will also show us what the 'database.yml' file looks like

###Do More

>Open your text file again and repeatedly copy-paste the text so that it's about 50-100 lines long.

I just opened the file up in RubyMine by using `mine ex12.txt`, and then copy and pasted a whole bunch and saved the file.

>Copy it to your temp directory again so you can look at it.
 Now do the exercise again, but this time page through it. On Unix you use the spacebar and w (the letter w) to go down and up. Arrow keys also work. On Windows just hit spacebar to page through.

`less ex12.txt` shows one page of the file.  The space bar pages down and the 'w' key pages back up.  They arrow keys <br/>
also move up or down one line at a time.

>Look at some of the empty files you created too.

When using the `less` or `more` commands on an empty file don't display anything, as would be expected.<br/>
the `more` command simply outputs nothing and gives you another prompt.  The `less` command on the other hand opens up<br/>
the file viewer, but there just isn't any content to display besides the filename. ('q' returns you to the prompt).

*The cp command will overwrite files that already exist so be careful copying files around.*
