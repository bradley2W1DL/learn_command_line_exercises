##Chapter 18 readme

**Alternative "english" ways of asking you to search files:**

>Show me the lines in foo.txt that have "ERROR" in them.

typing: `grep ERROR foo.txt` will print out all the lines within foo.txt with "ERROR" in them.

>Show me the lines in bar.txt that have "davinci" in them.

`grep davinci bar.txt` => prints out all the lines of bar.txt that contain "davinci" (this search was case-sensitive).

>Can you print all the lines in text files that have your first and last name in them?

Yea: `grep -i "bradley berger" *.txt`

*I have a question here that I haven't quite been able to figure out.  How can I search recursively through a directory<br/>
tree for my specific search term in all the text files?  I'll keep working on this and try to figure it out.*

I think I figured out a way to do this where I can search through all of my files for .txt files and then search<br/>
through all of those for my name and print the result into a new file...

`find ~/ -name "*.txt" | xargs grep "Bradley Berger" > name_game.txt`

The first part of this command uses find to look for all the .txt files in my root directory.  It then passes the <br/>
results to the right side of the pipe where the `xargs` command runs each individual result through the grep command, <br/>
searching for the string "Bradley Berger".  It then writes all of the files in which it found this string into the <br/>
'name_game.txt' file.  So if you view name_game you will see every text file in which that specific string can be found.

###Do More

>Use quotes to find "new file" and "old file" and "This is".

the commands for the above would be...<br/>
* `grep "new file" *.txt`
* `grep "old file" *.txt`
* `grep "This is" *.txt`

>Take the list of videos you created (or any other list) and use it to find some videos you want to find.

Within that list of of videos (I put that into a file named SOMEFILE.txt) I'll search for all the video files that I have <br/>
in the 'DaVinci Videos/in_class' folder with the following command:

`grep -i "davinci videos/in_class" SOMEFILE.txt`

This returned:<br/>
```
/Users/bird//workspace/DaVinci Videos/in_class/agile_introduction.mp4
/Users/bird//workspace/DaVinci Videos/in_class/build_your_brand_wordpress_intro.mp4
/Users/bird//workspace/DaVinci Videos/in_class/command_line_tracker_warmup.mp4
/Users/bird//workspace/DaVinci Videos/in_class/command_line_updates.mp4
/Users/bird//workspace/DaVinci Videos/in_class/git_101.mp4
/Users/bird//workspace/DaVinci Videos/in_class/git_102.mp4
/Users/bird//workspace/DaVinci Videos/in_class/intro_to_mentorship.mp4
/Users/bird//workspace/DaVinci Videos/in_class/learn_command_line.mp4
/Users/bird//workspace/DaVinci Videos/in_class/pair_programming.mp4
/Users/bird//workspace/DaVinci Videos/in_class/toolbelt_intro.mp4
/Users/bird//workspace/DaVinci Videos/in_class/tracker_intro.mp4
```

The command actually printed out all the files in that SOMEFILE.txt has listed as in the 'in_class' folder, <br/>
but since SOMEFILE.txt is just a list of .mp4 files the 'grep' search returned me all the videos that I was looking for.

*Unix: You can use -i to ignore case with grep. Try grep -i new *.txt

The '-i' option for `grep` stands for ignore-case. this means that will search for the designated string passed to it<br/>
without worrying about case.  -- By default, `grep` is case sensitive.
